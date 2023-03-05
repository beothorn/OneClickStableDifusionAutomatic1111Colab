# One click Automatic1111

If you want to play around with the image generating AI stable diffusion you cn follow this guide. If you just wan to start it already, jump to the How section below.

# What

This is just a launcher for [AUTOMATIC1111](https://github.com/AUTOMATIC1111/stable-diffusion-webui) stable diffusion web ui using google colab.  
[AUTOMATIC1111](https://github.com/AUTOMATIC1111/stable-diffusion-webui) is currently the best web ui to work with stable diffusion.  
This launcher runs in a single cell and uses google drive as your disk. This means your generations are saved to gdrive and next time you run it, it will not redownload anything, so it should start faster.  
Also a random password is generated on each run, which makes it safer from getting hijacked by bots scanning gradio urls.  

# Who is who, what is what

This is a very small and mostly too simple explanation of the things related to stable diffusion.

## Machine learning

Artificial intelligence and machine learning are very broad concepts. The kind of machine learning that is making the news and revolutionizing content creation are neural networks.  
Don't let the name fool you though, they are just a single math function that takes an input and produces an output, and there is a lot of constants inside it.  
What is called training is basically getting a database of inputs and expected outputs, running this function over the input, measuring the difference between what came out of the function and what was expected and the tweaking all constansts inside the function so the output is closer to the expected output.  
The model, the thing you download, is a file (or several files) containing those constants.  
The main take away from this is, AI is just a huge single function that needs a bunch of constants inside.  

## Stable diffusion

An AI that learned how to remove noise from images. Trained by taking an image, adding some noise and then using the noise image as input and the clear image as expected output. It also used an image already with noise, added even more noise and trained the AI with this, so the AI just tries to remove a little bit of noise per step.  
But when you add any image it always tries to denoise it, and that is how it generates images. It is like when you look at the clouds and see shapes when there is nothing actually there.  

## StableAI

The company  that trained stable diffusion and released it for free. They have a paid online editor [dreamstudio](https://beta.dreamstudio.ai)

## HuggingFace

A company that offers something like a github but for AI. You can host models, datasets and other things there. They also provide a library (transformes library) that make it suer simple to use the models (and other things) they are hosting.  

## Google colab

Google has a service, including a free tier, where you can run code on machines with powerfull gpus.  
Code is run using python notebooks.  
 
## AUTOMATIC1111

This is a developer that created an web ui for stable diffusion. This is the ui adopted by most of the community. There are others, but tis is by far the most active.  
 
# How

You will need a google account.  
Create an account at [huggingface](https://huggingface.co)  
Create a token at [https://huggingface.co/settings/tokens](https://huggingface.co/settings/tokens)  
Go to settings  
![Settings menu](https://github.com/beothorn/OneClickStableDifusionAutomatic1111Colab/raw/main/hfSettings.png)  
Create a new token  
![Create token](https://github.com/beothorn/OneClickStableDifusionAutomatic1111Colab/raw/main/hfToken.png)  
Copy the token and run this colab, you will need to give it permission to access google drive.  
The first run will take a long time as it will download the models on your gdrive.  
The next time it will be faster, but still take a couple of minutes.  
Rule of thumb, check if the console says downloading or shows a percentage.  
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/beothorn/OneClickStableDifusionAutomatic1111Colab/blob/main/StableDifusionAutomatic1111.ipynb)  
![Run colab](https://github.com/beothorn/OneClickStableDifusionAutomatic1111Colab/raw/main/colabRun.png)  
Copy the password from the console.  
![Copy password](https://github.com/beothorn/OneClickStableDifusionAutomatic1111Colab/raw/main/colabUserPass.png)  
Click on the link  
![Click the link](https://github.com/beothorn/OneClickStableDifusionAutomatic1111Colab/raw/main/colabLink.png)  
Use the user as user and the password you copied from the console.  
![Log in](https://github.com/beothorn/OneClickStableDifusionAutomatic1111Colab/raw/main/gradioLogin.png)  
You should then see the webui  
![This is cool](https://github.com/beothorn/OneClickStableDifusionAutomatic1111Colab/raw/main/webUi.png)
