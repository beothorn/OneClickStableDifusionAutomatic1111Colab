# One click Automatic1111

This is just a launcher for [AUTOMATIC1111](https://github.com/AUTOMATIC1111/stable-diffusion-webui) using google colab.

[AUTOMATIC1111](https://github.com/AUTOMATIC1111/stable-diffusion-webui) is currently the best web ui to work with stable diffusion.

This launcher runs in a single cell and uses google drive as your disk. This means your generations are saved to gdrive and next time you run it, it will not redownload anything, so it should start faster.

Also a random password is generated on each run, which makes it safer from getting hijacked by bots scanning gradio urls.

# How

Create an account at [huggingface](https://huggingface.co)

Create a token at [https://huggingface.co/settings/tokens](https://huggingface.co/settings/tokens)

Copy the token and run this colab, give it permission to access google drive.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/beothorn/OneClickStableDifusionAutomatic1111Colab/blob/main/StableDifusionAutomatic1111.ipynb)

Copy the password from the console.

Open the link printed (something like https://12345.gradio.app) on the console, log in with "user/generated password" and have fun!!
