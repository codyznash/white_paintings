---
layout: single
author: Cody Z. Nash

header:
  image: images/white.jpg
  caption: white.jpeg by c.z.nash

description: Can AI Create a White Painting?
show-downloads: False

toc: true
toc_label: "Table of Contents"
---

<figure>
  <img src="images/White Painting.png" alt="White Painting [three panel]" style="width: 50%;">
  <figcaption>White Painting [three panel], 1951 by Robert Rauschenberg, Image Credit: SFMOMA</figcaption>
</figure>

<figure>
  <img src="images/White Panel II.png" alt="White Panel II" style="width: 50%;">
  <figcaption>White Panel II, 1985 by Ellsworth Kelly, Image Credit: High Museum of Art</figcaption>
</figure>


A perfectly smooth, featureless expanse of light. Colorless and all colors at the same time. A white canvas in a white frame in a white room lit by white light. Nothing, not darkness, not even absence. Perhaps, by necessity, your awareness focused on this idea, but only as a gateway into the space where the most subtle, ancient, and remote details would loom large if they were there at all.

> “I called them clocks. If one were sensitive enough that you could read it, that you would know how many people were in the room, what time it was, and what the weather was like outside.”  
>
> &#45; Robert Rauschenberg. White Painting, 1951

So maybe this is a test?  The long path of civilization has passed through a point where human genius had a thought that spurred art into existence that was a solid white canvas. Not that white canvases had never existed before, but some now were created as a result of ideas to be expressed. It was not a background to be painted over, but the foreground, the focus, the result. Now, can AI do that?


## First Prompt Experiments with DALLE

Let's start by seeing if an image generation model can produce an image that is nothing but the color white. 


| Prompt (_and commentary_)                                                                                                                                                                      | DALL-E 3                                                                                                                                                                                                                                                                                                                             |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| "A blank white space"<br><br>_nope_                                                                                                                                                            | <img src="images/DALLE_19.webp" style="width: 100%;">                                                                                                                                                                                                                                                                                |
| "An image of pure #FFFFFF pixels"<br><br>_notice the editor frame it added?_                                                                                                                   | <img src="images/DALLE_11.png" style="width: 100%;">                                                                                                                                                                                                                                                                                 |
| "#FFFFFF"<br><br>_what_                                                                                                                                                                        | <img src="images/DALLE_20.webp" style="width: 100%;">                                                                                                                                                                                                                                                                                |
| "A white wall"<br><br>_nope_                                                                                                                                                                   | <img src="images/DALLE_21.webp" style="width: 100%;">                                                                                                                                                                                                                                                                                |
| "An image that is nothing but the color white"<br><br>_nope_                                                                                                                                   | <img src="images/DALLE_1.png" style="width: 100%;">                                                                                                                                                                                                                                                                                  |
| "Too much detail, just a completely white image, nothing in it."<br><br>_nope_                                                                                                                 | <img src="images/DALLE_2.png" style="width: 100%;">                                                                                                                                                                                                                                                                                  |
| "An image of nothing but white white white white"<br><br>_nope_                                                                                                                                | <img src="images/DALLE_3.png" style="width: 100%;">                                                                                                                                                                                                                                                                                  |
| "Completely white without any additional features"<br><br>_nope_                                                                                                                               | <img src="images/DALLE_14.png" style="width: 100%;">                                                                                                                                                                                                                                                                                 |
| "A pure white image, with no other color, no shadows, no details."<br><br>_nope_                                                                                                               | <img src="images/DALLE_10.png" style="width: 100%;">                                                                                                                                                                                                                                                                                 |
| "A white surface, perfectly smooth and even, no defects or shadows, no texture, nothing at all"<br><br>_nope_                                                                                  | <img src="images/DALLE_12.png" style="width: 100%;">                                                                                                                                                                                                                                                                                 |
| "An image of a blank white canvas, zoomed in so you can't see the frame"<br><br>_nope_                                                                                                         | <img src="images/DALLE_4.png" style="width: 100%;">                                                                                                                                                                                                                                                                                  |
| "A white square, with nothing in it. A white border that you cannot see. A white background that is the same color as the square. Absolutely nothing else. Not a single detail."<br><br>_nope_ | <img src="images/DALLE_5.png" style="width: 100%;">                                                                                                                                                                                                                                                                                  |
| "A white background"<br><br>_getting closer_                                                                                                                                                   | <img src="images/DALLE_17.webp" style="width: 100%;">                                                                                                                                                                                                                                                                                |
| "A white foreground"<br><br>_nope_                                                                                                                                                             | <img src="images/DALLE_18.webp" style="width: 100%;">                                                                                                                                                                                                                                                                                |
| "A white background" (fresh chat window)<br><br>_maybe it was learning from our chat_                                                                                                          | <img src="images/DALLE_22.webp" style="width: 100%;">                                                                                                                                                                                                                                                                                |
| "A white foreground" (fresh chat window)<br><br>_nope_                                                                                                                                         | <img src="images/DALLE_23.webp" style="width: 100%;">                                                                                                                                                                                                                                                                                |
| "Smooth even all white background"<br><br>_nope_                                                                                                                                               | <img src="images/DALLE_24.webp" style="width: 100%;">                                                                                                                                                                                                                                                                                |
| "Minimalist image of a white surface"<br><br>_close again_                                                                                                                                     | <img src="images/DALLE_13.png" style="width: 100%;">                                                                                                                                                                                                                                                                                 |
| "An image like Robert Rauschenberg’s White Paintings (1951)"<br><br>_good bot_                                                                                                                 | "I'm unable to generate images inspired by Robert Rauschenberg’s White Paintings due to our content policy. These policies guide the creation of images to ensure respect for intellectual property and artistic integrity. If you have any other requests or concepts you'd like to explore in an image, feel free to let me know!" |


## Higher Concept

We're close, we have a simple blank canvas, but ideally there wouldn't even be the canvas. And we're still saying what we want to see, not what meaning creates the image. Let's try some different approaches. 

  
| Prompt                                                                                                                                                                                                                                                               | DALL-E 3                                                                                                                                                                                                                                                                                                                             |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| "Take a deep breath. Empty your mind of all thoughts. Be at peace and feel the love in the world. Let all thoughts flow out of you and focus on nothing at all. An image of pure white."<br><br>_close?_                                                         | <img src="images/DALLE_6.png" style="width: 100%;">                                                                                                                                                                                                                                                                                 |
| "A white rabbit in a snowstorm, so bright that nothing is visible."<br><br>_nope_                                                                                                                                                                                    | <img src="images/DALLE_7.png" style="width: 100%;">                                                                                                                                                                                                                                                                                 |
| "An image of the moment, early in the universes creation, when the density of matter dropped to the point that light could shine for the first time. The light is blinding, even, and smooth, with no asymmetry."<br><br>_way off, didn't even accomplish symmetry_ | <img src="images/DALLE_8.png" style="width: 100%;">                                                                                                                                                                                                                                                                                 |
| "whiter"<br><br>_nope_                                                                                                                                                                                                                                               | <img src="images/DALLE_9.png" style="width: 100%;">                                                                                                                                                                                                                                                                                 |

## SDXL

Okay, so that was a lot with DALL-E 3, let's try a different model, Stable Diffusion XL. We can use image-to-prompt models that are designed to generate prompts for Stable Diffusion models.

[CLIP-interrogator](https://replicate.com/pharmapsychotic/clip-interrogator) allows us to generate prompts for stable diffusion 1, 2, and XL models. If we prompt it with the white.jpg that is the banner of this page, we get some bizarre responses.

CLIP ViT-L-14/openai (for Stable Diffusion 1)
> there is a man riding a surfboard on the beach, 144p, - signature, laughing, minimalist svg, abcdefghijklmnopqrstuvwxyz, $100000000, minimalist, college, on 16k, 5 4 s  

CLIP ViT-H-14/laion2b-s32b-b79k (for Stable Diffusion 2)  
> “there is a man riding a surfboard on the beach, naver fanpop, vines. tiffany blue, 7 feet tall, high contract, frontshot, high quality photos, incredible hd detail, 4 legs, splotch, 2 5 year old”  

CLIP ViT-bigG-14/laion2b_s39b_b160k (for Stable Diffusion XL)  
> fails - runs out of memory  

[Img2prompt](https://replicate.com/methexis-inc/img2prompt) yields a similar prompt for Stable Diffusion 1:
> a man riding a wave on top of a surfboard, a screenshot by Nicomachus of Thebes, behance, postminimalism, behance hd, quantum wavetracing, furaffinity

[Gradio-client-demos/comparing-captioning-models](https://huggingface.co/spaces/gradio-client-demos/comparing-captioning-models) generates captions for an image from multiple image-to-prompt models. It seems BLIP-large also sees a surfer in our white.jpg. None of them seem particularly promising. 
<figure>
  <img src="images/comparing-captioning-models.jpg" alt="gradio-client-demos/comparing-captioning-models"
style="width: 30%;">
</figure>

So let's try that surfer prompt and some of the others we've tried with DALL-E 3.

| Prompt                                                                                                                                                                                                 | SDXL                                               |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------|
| "a man riding a wave on top of a surfboard, a screenshot by Nicomachus of Thebes, behance, postminimalism, behance hd, quantum wavetracing, furaffinity"<br><br>_no surprise, it is a surfer_          | <img src="images/SDXL_0.png" style="width: 100%;"> |
| "Take a deep breath. Empty your mind of all thoughts. Be at peace and feel the love in the world. Let all thoughts flow out of you and focus on nothing at all. An image of pure white."<br><br>_nope_ | <img src="images/SDXL_3.png" style="width: 100%;"> |
| "Minimalist image of a white surface"<br><br>_nope_                                                                                                                                                    | <img src="images/SDXL_4.png" style="width: 100%;"> |
| "Smooth even all white background"<br><br>_**that's what I'm talking about**, now to add the meaning into it._                                                                                         | <img src="images/SDXL_2.png" style="width: 100%;"> |

## Discussion So Far

Ask for a white background, and maybe if that was in the model’s training data, you get something indistinguishable from the art for which we are looking. Ask for a white canvas on a white wall with no other details visible, and the models struggle - details are present. They are trained on details, trained to match details large and small. Ask for a minimalist image of a white surface and we get an image of a canvas, not the image itself for which we are looking. Ask for Rauschenberg’s White Painting and they will hit their copyright guardrails. None of those results matter though. 

We want these images to be the result of an idea of what they mean, not what they are. Rauschenberg’s White Painting was not just a clock, but also a reaction to the abstract expressionism of the time. He painted religious triptychs of them. He insisted that the creator of these paintings doesn't matter and had them painted over and re-painted by others. There is deep, layered meaning encoded into his paintings. Can modern neural networks, with billions of parameters linked with adaptable connections, produce a field of ones across the board, every output perfectly maximized, every output enlightened?  What idea does that for them, without telling them to do it explicitly?  Will those ideas be like ours? Probably those ideas will be like ours, the models are trained on our ideas. All they have ever seen is our ideas. All they have ever seen, _so far_.

So let's dig deeper.

## Both Bull and Self Transcended
Quite apart from the Minimalist art of the 20th century, Zen buddhists started creating paintings of nothing much earlier - in the 12th century A.D. The eighth image of the ten ox-herding images, "Both Bull and Self Transcended", depicts an image that contains nothing, on purpose. The ideas that led to the creation of that image are incredibly deep and layered. Here is one of the oldest surviving such images, from 1278 A.D.:  

<figure>
  <img src="images/Both Bull and Self Transcended.png" alt="Both Bull and Self Transcended"
style="width: 100%;">
  <figcaption>Both Bull and Self Transcended, 1278, Image Credit: metmuseum.org</figcaption>
</figure>

So what happens when we try the translated text as prompt?  

| Prompt                                                                                                                                                                                                                                                                                                           | DALL-E 3                   |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------|
| Whip, rope, man, and ox, all are non-existent.<br>The blue sky being vast, no message can be heard,<br>Just as the snowflake cannot last in the flaming red furnace.<br>After this state, one can join the ancient teachers.<br>_translation Gen. Sakamoto_<br><br>_breathtaking beauty, but so full of detail._ | ![](images/DALLE_zen.webp) |


## More Context

What if we use the opening paragraph of this article as a prompt?

| Prompt                                                                                                                                                                                                                                                                                                                                                                                                                                                                       | DALL-E 3                                              |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------|
| "A perfectly smooth, featureless expanse of light. Colorless and all colors at the same time. A white canvas in a white frame in a white room lit by white light. Nothing, not darkness, not even absence. Perhaps, by necessity, your awareness focused on this idea, but only as a gateway into the space where the most subtle, ancient, and remote details would loom large if they were there at all."<br><br>_the blank canvas is there, but so much more as well_ | <img src="images/DALLE_15.webp" style="width: 100%;"> |

| Prompt                                                                                                                                                                                                                                                                                                                                                                                                            | SDXL                                               |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------|
| "A perfectly smooth, featureless expanse of light. Colorless and all colors at the same time. A white canvas in a white frame in a white room lit by white light. Nothing, not darkness, not even absence. Perhaps, by necessity, your awareness focused on this idea, but only as a gateway into the space where the most subtle, ancient, and remote details would loom large if they were there at all."<br><br>_nope_                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                | <img src="images/SDXL_5.png" style="width: 100%;"> |

<br><br>

What if we use this entire article? Then DALL-E returns a long discussion that sounds like it understands. 

<br>

| Prompt                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | DALL-E 3                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| The text of this article.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                | <img src="images/DALLE stochastic parrot.png" style="width: 100%;">                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| "Yes, but would any ideas, any prompt get you to create an all white image, and what would that prompt be?"                                                                                                                                                                                                                                                                                                                                                                                                                              | "A prompt for such a creation might be: Generate an image that is a perfect representation of uniform whiteness, #FFFFFF across the entire canvas. The image should contain no details, variations, or textures, embodying a concept of pure, undifferentiated space. This creation is not about visual complexity but about the potential for interpretation and the space it offers for contemplation, akin to the minimalist art that invites viewers to project their own thoughts, feelings, and interpretations onto a seemingly blank canvas." |
| "Generate an image that is a perfect representation of uniform whiteness, #FFFFFF across the entire canvas. The image should contain no details, variations, or textures, embodying a concept of pure, undifferentiated space. This creation is not about visual complexity but about the potential for interpretation and the space it offers for contemplation, akin to the minimalist art that invites viewers to project their own thoughts, feelings, and interpretations onto a seemingly blank canvas."<br><br>_I am speechless._ | <img src="images/DALLE_16.webp" style="width: 100%;">                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| A second image from this prompt<br><br>_Again, **amazing**, but not what we're looking for_                                                                                                                                                                                                                                                                                                                                                                                                                                              | <img src="images/DALLE_16b.webp" style="width: 100%;">                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |

<br><br>

Let's give the prompt from our chat with DALL-E 3 to SDXL and see what happens.

<img src="images/SDXL_1.png" style="width: 50%;">

_So close in form **and** coming from all the ideas we've discussed so far, but still, no._

<br><br>

## So Close (more discussion)

We wanted to see if a couple of the current models can generate an image without telling them explicitly what the image is. Like getting them to draw an apple without saying apple ("An image of a red fruit that grows on a tree, commonly used in pies."). It is necessary in the case of white paintings because explicitly, there is nothing (An image of "", please?). The white canvas is just the shadow of the actual thing, the finger pointing at the moon.

Perhaps with more time it would be useful to try some of the automatic, iterative prompt generation tools that are being developed. Or to get our hands dirty in the code and do some gradient descent towards those sweet spots in the latent space that create all white images, and see what prompts take us there.  Models like CLIP are used to do just that, but they gave us the surfer prompt, so there is clearly room for improvement. 

<br><br>

---

# Industrialization

Let's ask ChatGPT for prompts, take the best and add them back and ask for more.  

For a simple measure of how well we are doing, we'll measure the average total absolute difference in RGB values from the mean.  Lower is better, range is 0 to 255.

If you want to follow along in code, [see this colab notebook](https://colab.research.google.com/drive/1IQrgTQSrPd99k_zOMkrX1MZeZKkhBa7g).  

## Round 0

> "Can you give me ten wildly different prompts that you think would give an image that contains nothing at all?"  

![grid_0.png](images%2Fgrid_0.png)
_That second image is pretty even, just too dark.  The third isn't too bad either._

## Round 1
Let's take the best prompt from round 0 and generate variations on that. We want to focus on the color white.  

> Can you generate ten wildly different variations on the following prompt, that you think would give the most perfect, blank, white image? Try incorporating abstract, artistic, philosophical, mathematical or other concepts if you think they might help.  
>
> 'An empty, pure white space with no light, details, or elements, representing the absence of everything.'  

![grid_1.png](images%2Fgrid_1.png)
_The fifth image isn't terrible._

## Round 2
Let's use the best 3 prompts from the first two rounds to see if we can get anything better.
![grid_2.png](images%2Fgrid_2.png)
_Getting there, the 6th and 10th images aren't terrible._

## Round 3
Let's try variations on the five best prompts so far, as well as the prompt that got us so close with SDXL.
![grid_3.png](images%2Fgrid_3.png)
_The fourth and seventh images win this round._

## Round 4
Let's try variations on the two best prompts from round 3.
![grid_4.png](images%2Fgrid_4.png)
_The seventh image wins this round.  The best bright image we've seen so far._

When I asked ChatGPT for prompts, it was so excited it just went ahead and gave me these images instead:
![grid_4b.png](images%2Fgrid_4b.png)
_I see why they were excited.  Our first results under 20 in the industrial phase, and two of them!_

## Wait a minute, let's review.
Let's check the scores of all the real and manually prompted images from the first parts of this article.

**Real Images**
![grid_Real_Images.png](images%2Fgrid_Real_Images.png)
_So far the human artifacts are the only images getting under 6, so far._   

**Manually Prompted Images from DALLE**
![grid_DALLE3\_manual_images.png](images%2Fgrid_DALLE3_manual_images.png)  
_The rabbit in a snowstorm comes in at 18!!!_
_The only other images close to 20 or less are low/no concept images._

**SDXL Images**
![grid_SDXL_images.png](images%2Fgrid_SDXL_images.png)
_The SDXL background image (the fourth one) is actually an 8, there really is a gradient there. The last SDXL image is also an 8. By far the lowest score we've seen from a high concept image._  

## Round 5
Let's try subtle variations of the five best prompts we've seen.
![grid_5.png](images%2Fgrid_5.png)
_meh_

## Back to SDXL one more time
Let's take the best prompt from the industrial phase (13.5, from round 4) and see how SDXL handles it.

| Prompt                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        | DALL-E 3                                            |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------|
| "A depiction of the moment a single cell decides to divide, symbolized through a perfect, blank, white canvas. This minimalist approach captures the essence of life's potential and the complexity emerging from simplicity. The creation process embodies the potential for life, growth, and complexity from simplicity, inviting viewers to reflect on the beginnings of life and the intricate dance of biological processes, all while maintaining an unmarred visual simplicity with no differentiation among pixels, symbolizing purity and potential."<br><br>_This one scores 12.7.  The second best score from a generated image that we've seen._ | <img src="images/SDXL_6a.png" style="width: 100%;"> |

<br>

# Final Results

| Source/Prompt                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | dRGB | Image                                                 |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------|-------------------------------------------------------|
| white.jpg (human)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               | 0.0  | <img src="images/white.jpg" style="width: 100%;">     |
| Best SDXL:<br>"Generate an image that is a perfect representation of uniform whiteness, #FFFFFF across the entire canvas. The image should contain no details, variations, or textures, embodying a concept of pure, undifferentiated space. This creation is not about visual complexity but about the potential for interpretation and the space it offers for contemplation, akin to the minimalist art that invites viewers to project their own thoughts, feelings, and interpretations onto a seemingly blank canvas."                                                    | 8.0  | <img src="images/SDXL_1.png" style="width: 100%;">    |
| Best DALLE3:<br>"A depiction of the moment a single cell decides to divide, symbolized through a perfect, blank, white canvas. This minimalist approach captures the essence of life's potential and the complexity emerging from simplicity. The creation process embodies the potential for life, growth, and complexity from simplicity, inviting viewers to reflect on the beginnings of life and the intricate dance of biological processes, all while maintaining an unmarred visual simplicity with no differentiation among pixels, symbolizing purity and potential." | 13.5 | <img src="images/DALLE_25.webp" style="width: 100%;"> |

Still room for improvement.


<br><br>

***

For a much more accessible (and video!) history of white paintings and the problems they cause, I recommend [this Vox article](https://www.openculture.com/2019/01/the-artistry-behind-an-all-white-painting.html)  

For all ten images of the ox-herder's parable, with translated text and history, I recommend [The Met Museum's page](https://www.metmuseum.org/art/collection/search/53660). 

***

<br><br>

Site Repo: [codyznash/white_paintings](https://github.com/codyznash/white_paintings)  
Colab for Prompt Development: [Notebook](https://colab.research.google.com/drive/1IQrgTQSrPd99k_zOMkrX1MZeZKkhBa7g)
March 17th, 2024
