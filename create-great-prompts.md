# How to Write Great Prompts in Stable Diffusion

Stable Diffusion is a software that uses AI to create images. To guide it to create the image you want, you can use positive and negative prompts. Positive prompts are words or phrases that tell the software what you want to see in the image, while negative prompts tell it what to avoid. 

Creating a good prompt is crucial. In fact, there are numerous websites where people seek ways to improve their prompt writing skills. This interest has given rise to a term called "prompt engineering.”

## 1. The Anatomy of a Prompt

In my experience, a prompt should incorporate specific elements to produce a high-quality image.

These include a subject, an artistic medium and style, the aesthetics of the image, and image quality. These elements collectively result in the following prompt formula:

```markdown
<Artistic medium> <Adjective> Subject <Action or Accessory> <Location> <Artistic style> <Aesthetics> <Image quality>
```

In this formula:

- All the elements enclosed in angle brackets <...> are optional. This means you can choose whether or not to include them in your prompt.
- The only mandatory element is the **subject**, so you must include it to describe the main focus of your image.
- The arrangement of elements is flexible, enabling you to position adjectives, actions, location, aesthetics, and image quality either before or after the subject. This lets you to tailor your prompt to align with the context or your personal style.

To gain a deeper understanding of each of these elements, we will gradually construct our prompt formula step-by-step:

-  [**Step 1**: The subject](/prompt-formula/01-prompt-formula-subject.md)
-  [**Step 2**:Artistic Medium](/prompt-formula/02-prompt-formula-medium.md)
-  [**Step 3**:Artistic Style](/prompt-formula/03-prompt-formula-style.md)
-  [**Step 4**:Aesthetics](/prompt-formula/04-prompt-formula-aesthetics.md)
-  [**Step 5**:Image quality](/prompt-formula/05-prompt-formula-quality.md)

## 2. Using Weights in Your Prompts

Weights for prompts are a way of controlling how much influence each word or phrase has on the image generation process. By adding parenthesis and a weight number to a word or phrase, you can increase or decrease its importance. 

For example, if you want to generate an image of a monkey holding ice cream, you can use the prompt "monkey holding ice cream". However, if you want to emphasize the beer more, you can use the prompt "monkey holding (ice cream: 1.5)". 

Conversely, if you want to de-emphasize the ice-cream, you can use the prompt "monkey holding (ice cream: 0.5)".

The weighting system operates within a range of -1 to 1, where 0 is the default weight and 1 is the maximum weight. You can use parentheses to group words or phrases together and apply weights to them. 

For example, if you want to generate an image of a monkey holding ice cream in the style of Vincent Van Gogh, you can use the prompt "monkey holding ice cream (in the style of Vincent Van Gogh: 1.2)". This will increase the weight of the phrase "in the style of Vincent Van Gogh" and make the image resemling more the style of a Van Gogh Painting. 

You can also use nested parentheses to combine weights. For example, if you want to generate an image of a monkey holding ice cream in the style of Vincent Van Gogh, but with more emphasis on the beer, you can use the prompt "monkey holding (a beer:1.4) (in the style of Vincent Van Gogh:1.1)". This will increase the weight of both the word "beer" and the phrase "in the style of Vincent Van Gogh", but more so for the former.

Prompt weighting is a powerful tool that allows you to fine-tune the image generation process and achieve more creative and diverse results. However, it also comes with some risks and limitations. For instance, using too high or too low weights can result in lower quality images or unexpected outcomes. Moreover, some words or phrases may have stronger or weaker effects than others, depending on the model's knowledge and preferences. Therefore, it is advisable to experiment with different weights and see how they affect the image output. You can also use negative prompts to exclude unwanted elements from the image.


## 3. Negative Prompts

Negative prompts serve to specify what the image should avoid containing, helping you in steering clear of undesired elements or reducing ambiguity in image generation. For instance, to generate an image of a bustling city at night without people, use the negative prompt "people". 

You can also apply weights to your negative prompts to emphasise elements that you don't want in you image. 

You might wonder: Why have a positive prompt and a negative prompt? Why not include things to avoid in the positive prompt?

The reason for separating positive and negative prompts is to provide clearer instructions to the model. Mixing them can confuse the model, making it more challenging to generate the desired image. By using positive prompts to specify what you want and negative prompts to specify what you don't want, you offer the AI model distinct instructions, leading to improved results.

## 4. Other Factors Affecting your Prompt

Now that you understand how to construct a prompt — utilizing a prompt formula, incorporating weights, and employing negative prompts — yet your image doesn't quite match your vision, what's the issue? What can you do?

Several influencing factors come into play in how the image is generated, irrespective of how skillfully you formulate your prompt.

- **The model:** The model you pick for making images is crucial for what you create. For instance, if you use a super specific model tuned for Anime, it might not be great at making realistic photos. Always be mindful of the model you choose. You can find more info on models in my detailed explanation here.
- **Add-ons:** With Stable Diffusion, you can use extensions that impact how your images turn out. Here are a few examples:
    - **LoRA models:** These are small neural networks specialized in generating specific details like faces, hands, or clothing. Boost your Stable Diffusion results by applying them to a compatible model.
    - **Refiners:** Specialized models for the final denoising steps in the diffusion process. Apply them to the generated latents from the base model, using the same text prompt, for sharper and more realistic images.
    - **ControlNet:** This extension lets you control the pose, color, and content of your images using a reference image. Whether mimicking an existing style or crafting custom images, ControlNet gives you more flexibility and precision.

## 5. Final Thoughts

When generating images using AI, providing a good prompt is essential for obtaining desired results. Here are some rules and tips for describing a good prompt:

1. **Be Clear and Specific:** Clearly articulate what you want in the image. Use specific details and avoid ambiguity.

2. **Include Key Elements:** Mention important elements, objects, or characteristics you want in the image. This helps the AI understand your expectations.

3. **Consider Style and Mood:** Describe the desired style or mood for the image. Specify if you want it realistic, surreal, colorful, etc.

4. **Use Descriptive Language:** Utilize vivid and descriptive language to convey your vision. Paint a clear picture with words.

5. **Experiment and Iterate:** If the initial result is not what you want, iterate and experiment with different phrasings or additional details in your prompt.

6. **Provide Context:** Give context or background information if needed. This helps the AI understand the scene or scenario you have in mind.

7. **Use Reference Images:** If applicable, provide reference images or examples to illustrate your vision better.

8. **Avoid Ambiguity:** Minimize ambiguous terms or conflicting instructions. The more precise, the better.

9. **Consider Composition:** Describe the arrangement of elements in the image. Specify the composition and spatial relationships.

10. **Experiment with Parameters:** Some AI models allow you to tweak parameters. Experiment with these to fine-tune the output to your liking.

Remember, the effectiveness of the prompt may depend on the specific AI model or platform you are using. It's often helpful to review the guidelines provided by the AI service you're working with to understand how to formulate prompts effectively.

> **Pro Tip:** Continue experimenting, combining different elements, and consistently seek new ways to enhance your prompts. Gain insights from others, perhaps by exploring platforms like [Prompt Hero](https://prompthero.com/) on the internet. In my experience, [Leonardo.AI](https://leonardo.ai/) stands out as one of the finest websites for prompt learning. Not only does it provide an excellent AI image generation tool, but it also features a wealth of community images, allowing you to observe what prompts people used and learn from their approaches. To find additional details about Leonardo AI, check out the [playlist](https://www.youtube.com/playlist?list=PL-J5F8ezBp9CzhYTimE42C3oGiChRxp8_) I curated on YouTube.





