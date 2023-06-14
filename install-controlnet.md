# ControlNet Installation Guide for AUTOMATIC1111 Web UI

1. Open Stable Diffusion Web UI. For more details, please see [this page](sd-installation-guide.md#run-stable-diffusion-web-ui-on-mac).
2. Open the Extensions tab in Automatic1111 Webui, clicking on Install from URL, and entering `https://github.com/Mikubill/sd-webui-controlnet.git` as the URL for extension's git repository. Then click on Install and wait for a few seconds. Apply and restart UI after installation.
3. Download the ControlNet models from HuggingFace: `https://huggingface.co/lllyasviel/ControlNet-v1-1/tree/main`. You need to download the model files ending with `.pth` and put them in your `stable-diffusion-webui/extensions/sd-webui-controlnet/models` folder.
4. Restart Automatic1111 Webui completely. You should see the ControlNet models in the Model dropdown menu. You may need to refresh the page to see them.