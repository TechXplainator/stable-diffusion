# Running SDXL on Mac: Top Methods

## Why Run SDXL Locally?

- Data privacy
- More freedom - NSFW


## Shared RAM Issue on Mac

So, you've got a Mac, nice choice! But when it comes to using AI image generation tools locally on your mac, you may run into some issues. Why? Because AI image generators use VRAM and RAM to store and process data, but in different ways than other apps you run on your Mac.

VRAM is the memory of the graphics card, which is specialized for handling graphical data and operations. It is usually faster and more efficient than regular RAM, which is the memory of the computer system, which stores and transfers data for various applications and processes.



Basically, your MacBook Air M2 has both a central processing unit (CPU) and a graphics processing unit (GPU). The CPU is like the brain of your computer, handling all sorts of tasks like running programs and crunching numbers. The GPU, on the other hand, is specifically designed to handle graphics-related tasks, like rendering images and videos for games or design programs.

Now, when Apple says they share memory between the CPU and GPU, it means they use the same pool of memory for both of these processors to work with. Instead of having separate dedicated memory for the CPU and GPU, they both use the RAM (Random Access Memory) in your MacBook Air.

This setup can be pretty efficient because it allows the CPU and GPU to quickly access and share data without needing to constantly move it back and forth between separate memory pools. It's like having a big communal workspace where both the CPU and GPU can grab what they need to get their jobs done without stepping on each other's toes.

So, in a nutshell, sharing memory between the CPU and GPU in your MacBook Air M2 helps keep things running smoothly and efficiently, which is always a good thing!









Core ML is a framework that allows you to integrate machine learning models into your Mac app. Core ML provides a unified representation for all models, so you can use the same APIs and user data to make predictions, and to train or fine-tune models, all on your Mac device¹².

Core ML is designed to take advantage of the powerful hardware technology in Mac computers, such as the CPU, GPU, and Neural Engine. This helps to optimize the performance, memory, and power consumption of your app¹².

You can create and train Core ML models using the Create ML app in Xcode, or convert models from other machine learning libraries using Core ML Tools¹²³. You can also use Core ML to update your models with new data on your Mac device, which helps to personalize and improve your models without compromising privacy¹².

Core ML is the foundation for other frameworks and functionalities that use machine learning, such as Vision, Natural Language, Speech, and Sound Analysis¹². You can use these frameworks to perform tasks such as analyzing images, processing text, converting audio to text, and identifying sounds in audio¹².

Source: Conversation with Bing, 11/02/2024
(1) Core ML Overview - Machine Learning - Apple Developer. https://developer.apple.com/machine-learning/core-ml/.
(2) Core ML | Apple Developer Documentation. https://developer.apple.com/documentation/coreml.
(3) GitHub - apple/coremltools: Core ML tools contain supporting tools for .... https://bing.com/search?q=core+ml+mac.
(4) GitHub - apple/coremltools: Core ML tools contain supporting tools for .... https://github.com/apple/coremltools.
(5) Apple - CoreML | onnxruntime. https://onnxruntime.ai/docs/execution-providers/CoreML-ExecutionProvider.html.
(6) Releasing Swift Transformers: Run On-Device LLMs in Apple Devices. https://huggingface.co/blog/swift-coreml-llm.

## Honorable Mentions

A few honorable mentions that did not make the list, mainly because although they work great on Mac, these tools do not support SDXL. However, if you are looking for great AI image generators for older generation models, these could be great choices for you.

### Diffusion Bee

DiffusionBee is a free open source app that lets you generate and edit images using text prompts and AI tools. It provides an intuitive user interface for you that allows you to run stable diffusion models locally on your mac. 

The recommended hardware requirements for running DiffusionBee are:

- A Mac computer with Apple Silicon chip (M1 or M2) for optimal performance⁵⁷
- At least 16 GB of RAM for faster generation¹⁵⁷
- macOS 12.5.1 or higher⁵⁷

You can download DiffusionBee from its official website² or from GitHub⁶. You can also check out some tutorials and tips on how to use it³⁴.

Source: Conversation with Bing, 11/02/2024
(1) DiffusionBee - Stable Diffusion App for AI Art. https://diffusionbee.com/.
(2) "Diffusion Bee" Is the Easiest Way to Make AI Art on Mac - How-To Geek. https://www.howtogeek.com/832763/diffusion-bee-is-the-easiest-way-to-make-ai-art-on-mac/.
(3) Stable Diffusion PC Hardware Requirement: Detailed Guide - DC. https://decentralizedcreator.com/stable-diffusion-pc-hardware-requirement-detailed-guide/.
(4) DiffusionBee - Stable Diffusion App for AI Art. https://diffusionbee.com/download.
(5) How to use DiffusionBee - GitHub. https://github.com/divamgupta/diffusionbee-stable-diffusion-ui/blob/master/docs/DOCUMENTATION.md.
(6) How to Use Diffusion Bee to Run Stable Diffusion Locally?. https://aitoolmall.com/news/how-to-use-diffusion-bee/.
(7) DiffusionBee Review 2024: What It Is, How to Use It & Is It Worth It?. https://aihungry.com/tools/diffusionbee.
(8) undefined. https://t.co/wzUqpkIzKf.
(9) undefined. https://t.co/mVFQD0lUsi.
(10) undefined. https://t.co/kgTOYSAydz%29.
(11) undefined. https://avatars.githubusercontent.com/u/1890549?v=4.
(12) undefined. https://github.com/divamgupta/diffusionbee-stable-diffusion-ui/blob/master/docs/DOCUMENTATION.md?raw=true.
(13) undefined. https://desktop.github.com.
(14) undefined. https://docs.github.com/articles/about-issue-and-pull-request-templates.
(15) undefined. https://github.com/divamgupta/diffusionbee-stable-diffusion-ui/raw/master/docs/DOCUMENTATION.md.