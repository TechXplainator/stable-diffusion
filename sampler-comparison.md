# Comparison of Stable Diffusion Sampling Methods

## Configuration
* Model [v1-5-pruned-emaonly.ckpt](https://huggingface.co/runwayml/stable-diffusion-v1-5/resolve/main/v1-5-pruned-emaonly.ckpt)
* positive prompt: "profile photo fof a cute cat"
* No negative prompt
* CFG scale 7
* Seed 2961182060


# Comparison

| Sampler | 1 <br> Step | 5 <br> Steps | 10 <br> Steps | 15 <br> Steps | 20 <br> Steps | 25 <br> Steps | 30 <br> Steps | 35 <br> Steps | 40 <br> Steps | 45 <br> Steps | 50 <br> Steps | 55 <br> Steps | 60 <br> Steps|
| - | - | - | -| - | - | - | - | - | - | - | - | - | - |
| Euler a | ![00000-2961182060.png](images/sd-comparison/00000-2961182060.png) | ![00001-2961182060.png](images/sd-comparison/00001-2961182060.png) | ![00002-2961182060.png](images/sd-comparison/00002-2961182060.png) | ![00003-2961182060.png](images/sd-comparison/00003-2961182060.png) | ![00004-2961182060.png](images/sd-comparison/00004-2961182060.png) | ![00005-2961182060.png](images/sd-comparison/00005-2961182060.png) | ![00006-2961182060.png](images/sd-comparison/00006-2961182060.png) | ![00007-2961182060.png](images/sd-comparison/00007-2961182060.png) | ![00008-2961182060.png](images/sd-comparison/00008-2961182060.png) | ![00009-2961182060.png](images/sd-comparison/00009-2961182060.png) | ![00010-2961182060.png](images/sd-comparison/00010-2961182060.png) | ![00011-2961182060.png](images/sd-comparison/00011-2961182060.png) | ![00012-2961182060.png](images/sd-comparison/00012-2961182060.png) |
| Euler | ![00013-2961182060.png](images/sd-comparison/00013-2961182060.png) | ![00014-2961182060.png](images/sd-comparison/00014-2961182060.png) | ![00015-2961182060.png](images/sd-comparison/00015-2961182060.png) | ![00016-2961182060.png](images/sd-comparison/00016-2961182060.png) | ![00017-2961182060.png](images/sd-comparison/00017-2961182060.png) | ![00019-2961182060.png](images/sd-comparison/00019-2961182060.png) | ![00020-2961182060.png](images/sd-comparison/00020-2961182060.png) | ![00021-2961182060.png](images/sd-comparison/00021-2961182060.png) | ![00022-2961182060.png](images/sd-comparison/00022-2961182060.png) | ![00023-2961182060.png](images/sd-comparison/00023-2961182060.png) | ![00024-2961182060.png](images/sd-comparison/00024-2961182060.png) | ![00025-2961182060.png](images/sd-comparison/00025-2961182060.png) | ![00026-2961182060.png](images/sd-comparison/00026-2961182060.png) |
| LMS | ![00027-2961182060.png](images/sd-comparison/00027-2961182060.png) | ![00028-2961182060.png](images/sd-comparison/00028-2961182060.png) | ![00029-2961182060.png](images/sd-comparison/00029-2961182060.png) | ![00030-2961182060.png](images/sd-comparison/00030-2961182060.png) | ![00031-2961182060.png](images/sd-comparison/00031-2961182060.png) | ![00032-2961182060.png](images/sd-comparison/00032-2961182060.png) | ![00033-2961182060.png](images/sd-comparison/00033-2961182060.png) | ![00034-2961182060.png](images/sd-comparison/00034-2961182060.png) | ![00035-2961182060.png](images/sd-comparison/00035-2961182060.png) | ![00036-2961182060.png](images/sd-comparison/00036-2961182060.png) | ![00037-2961182060.png](images/sd-comparison/00037-2961182060.png) | ![00038-2961182060.png](images/sd-comparison/00038-2961182060.png) | ![00039-2961182060.png](images/sd-comparison/00039-2961182060.png) |
