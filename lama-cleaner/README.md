# About

> A free and open-source inpainting tool powered by SOTA AI model.
>
> [https://github.com/Sanster/lama-cleaner](https://github.com/Sanster/lama-cleaner)

The file `docker-compose-cpu.yml` configures the container to run on CPU, which is highly impractical for a few of the models. I configured it to use the FcF model by default because it produces good results and runs reasonably fast on CPU.

I don't have a supported Nvidia GPU to test this with, so I currently only provide a compose file for CPU.
