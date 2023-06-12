# ControlNet Installation Guide

- Install the OpenCV library by running 

`pip install opencv-python` 

in your terminal.
- Install the ControlNet extension by opening the Extensions tab in Automatic1111 Webui, clicking on Install from URL, and entering `https://github.com/Mikubill/sd-webui-controlnet.git` as the URL for extension's git repository. Then click on Install and wait for a few seconds.
- Download the ControlNet models from HuggingFace: `https://huggingface.co/lllyasviel/ControlNet-v1-1/tree/main`. You need to download the model files ending with `.pth` and put them in your `stable-diffusion-webui/extensions/sd-webui-controlnet/models` folder. You can also download some pre-trained models by TheAlly from Civitai: `https://civitai.com/models/9251/controlnet-models` or `https://civitai.com/models/9868/controlnet-models`.
- Restart Automatic1111 Webui completely, including your terminal. You should see the ControlNet models in the Model dropdown menu. You may need to refresh the page to see them.
