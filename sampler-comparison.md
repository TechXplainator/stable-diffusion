# Comparison of Stable Diffusion Sampling Methods

## Configuration
* Model [v1-5-pruned-emaonly.ckpt](https://huggingface.co/runwayml/stable-diffusion-v1-5/resolve/main/v1-5-pruned-emaonly.ckpt)
* positive prompt: "profile photo fof a cute cat"
* No negative prompt
* CFG scale 7
* Seed 2961182060


# Comparison

| Sampler / Steps | &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; 1 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; | 5 | 10 | 15 | 20 | 25 | 30 | 35 | 40 | 45 | 50 | 55 | 60 |
| --------------- | - | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
| Euler a | ![00000-2961182060.png](images/sd-comparison/00000-2961182060.png) | ![00001-2961182060.png](images/sd-comparison/00001-2961182060.png) | ![00002-2961182060.png](images/sd-comparison/00002-2961182060.png) | ![00003-2961182060.png](images/sd-comparison/00003-2961182060.png) | ![00004-2961182060.png](images/sd-comparison/00004-2961182060.png) | ![00005-2961182060.png](images/sd-comparison/00005-2961182060.png) | ![00006-2961182060.png](images/sd-comparison/00006-2961182060.png) | ![00007-2961182060.png](images/sd-comparison/00007-2961182060.png) | ![00008-2961182060.png](images/sd-comparison/00008-2961182060.png) | ![00009-2961182060.png](images/sd-comparison/00009-2961182060.png) | ![00010-2961182060.png](images/sd-comparison/00010-2961182060.png) | ![00011-2961182060.png](images/sd-comparison/00011-2961182060.png) | ![00012-2961182060.png](images/sd-comparison/00012-2961182060.png) |
