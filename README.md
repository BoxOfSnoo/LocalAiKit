# Local AI Kit

Some stuff to play around especially with AI & LLMs on local GPUs.

I tried to arrange this to give the repo multiple functions:

**llama-server**: I built a Docker image to use the turboquant version of llama-server in a docker image.  This image should watch the `models.ini` file and dynamically unload/reload the models when it changes.  This only seems to work if you use the `docker-compose up --watch` option (you can also run with `-d` I believe).  You need this dockerfile in the llama-cpp repo folder for it to work.  The `docker-cuda` folder is because this is tweaked for my RTX 3060 card right now, other nVidia cards will need to specify other CUDA library versions in the script.  Add the ROCm or SYCL (or whatever) versions as needed. 

**model-tweaks**: This is my models.ini right now.  I could split this into different models but this is under heavy tweakage at all times.  Still. Let's use git.

**prompts**: A bunch of prompts mostly designed to get consistent effort across models.

More folders may be added as they make sense.