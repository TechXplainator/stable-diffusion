# Comparison of Stable Diffusion Sampling Methods

## Configuration
* Model [v1-5-pruned-emaonly.ckpt](https://huggingface.co/runwayml/stable-diffusion-v1-5/resolve/main/v1-5-pruned-emaonly.ckpt)
* positive prompt: "profile photo fof a cute cat"
* No negative prompt
* CFG scale 7
* Seed 2961182060


# Comparison

| Sampler | 1 <br> Step | 5 Steps | 10 Steps | 15 Steps | 20 Steps | 25 Steps | 30 Steps | 35 Steps | 40 Steps | 45 Steps | 50 Steps | 55 Steps | 60 Steps|
| - | - | - | -| - | - | - | - | - | - | - | - | - | - |
| Euler a | ![00000-2961182060.png](images/sd-comparison/00000-2961182060.png) | ![00001-2961182060.png](images/sd-comparison/00001-2961182060.png) | ![00002-2961182060.png](images/sd-comparison/00002-2961182060.png) | ![00003-2961182060.png](images/sd-comparison/00003-2961182060.png) | ![00004-2961182060.png](images/sd-comparison/00004-2961182060.png) | ![00005-2961182060.png](images/sd-comparison/00005-2961182060.png) | ![00006-2961182060.png](images/sd-comparison/00006-2961182060.png) | ![00007-2961182060.png](images/sd-comparison/00007-2961182060.png) | ![00008-2961182060.png](images/sd-comparison/00008-2961182060.png) | ![00009-2961182060.png](images/sd-comparison/00009-2961182060.png) | ![00010-2961182060.png](images/sd-comparison/00010-2961182060.png) | ![00011-2961182060.png](images/sd-comparison/00011-2961182060.png) | ![00012-2961182060.png](images/sd-comparison/00012-2961182060.png) |
| Euler | ![00013-2961182060.png](images/sd-comparison/00013-2961182060.png) | ![00014-2961182060.png](images/sd-comparison/00014-2961182060.png) | ![00015-2961182060.png](images/sd-comparison/00015-2961182060.png) | ![00016-2961182060.png](images/sd-comparison/00016-2961182060.png) | ![00017-2961182060.png](images/sd-comparison/00017-2961182060.png) | ![00019-2961182060.png](images/sd-comparison/00019-2961182060.png) | ![00020-2961182060.png](images/sd-comparison/00020-2961182060.png) | ![00021-2961182060.png](images/sd-comparison/00021-2961182060.png) | ![00022-2961182060.png](images/sd-comparison/00022-2961182060.png) | ![00023-2961182060.png](images/sd-comparison/00023-2961182060.png) | ![00024-2961182060.png](images/sd-comparison/00024-2961182060.png) | ![00025-2961182060.png](images/sd-comparison/00025-2961182060.png) | ![00026-2961182060.png](images/sd-comparison/00026-2961182060.png) |
