# Tensorflow
Description: The basics of machine learning with tensorflow and basics of its usage.

- [Loading Jupyter Notebooks in Colab](#loading-jupyter-notebooks-in-colab)
- [Tensorflow Hello World : MNIST](#tensorflow-hello-world-mnist)
- [Where to go next?](#where-to-go-next)
  - [Further Examples](#further-examples)
    - [Tensorboard](#tensorboard)
    - [GPU vs CPU](#gpu-vs-cpu)
    - [Compute Resources](#compute-resources)
- [Debugging](#debugging)
  - [Tensorflow API Documentation](#tensorflow-api-documentation)
  - [Communities](#communities)

## Loading Jupyter Notebooks in Colab

For the sake of simplicity, we will be loading the colab notebooks for today's talk from this Github repo, but this can be done in several different ways.

First, go to colab.research.google.com. Assuming you are logged into drive, you will be prompted with a screen that gives you a choice of notebooks to load. If you're interested in learning more about the colab platform, the examples tab covers some great basics on configuring the environment. For now, click on github and enter the url github.com/OS2G as shown in the image below. It will automatically detect the repos which contain .ipynb files. Click the notebook titled "getting_into_the_flow_of_tensorflow.ipynb".

![How to Load the Notebook](newColabFromGithub.PNG)

## Tensorflow Hello World: MNIST
Once you have opened the notebook titled "Getting into the flow of tensorflow" from the Github repo, you will be able to see the details on tensorflow itself. You can also just click on the notebook from the repo itself, as Github does a passable job of visualizing Jupyter notebooks.

## Where to go next?
Now that we've shown how simple it is to run a basic ML task using tensorflow, let's take a look at where you can go next to learn more.

### Further Examples
Many people have published a wide range of .ipynb notebooks that do just about anything you can imagine. Google in particular has a slew of worthwhile tutorials that demonstrate different functionalities of tensorflow that can be found at https://www.tensorflow.org/guide/ .

#### Tensorboard
Understanding the structure and performance of a network can be challenging. Tensorboard is an incredibly useful tool which makes it simple to visually see both the structure of a network and how it performs over time. This tutorial explains the basics and showcases its utility in visualising results: https://www.tensorflow.org/tensorboard/get_started. 

#### GPU vs CPU
Another valuable feature of tensorflow is its GPU support. Tensorflow is extensively optimized to run on hardware. To see this in action, load up the Compare CPU to GPU Notebook from this repo. It's also worth noting that at the beginning of the file, we load Tensorflow Version 1.x, as this tutorial was made to run with the 1.14 API. This works when a whole script is built for the 1.0 API but other approaches are necessary for using a small piece of the 1.0 API in a file primarily using TF 2.0 . A more in-depth guide using TF 2.0 can be found [here](https://www.tensorflow.org/guide/gpu). 

#### Compute Resources
A key limitation with Machine Learning is compute resources. Colab is great for simple tasks but larger jobs will require larger amount of dedicated hardware, particularly if you want to iterate quickly. There are several paths you can take to upgrading the runtime you're using for tensorflow.
##### Run locally
If you have a powerful home PC with an Nvidia graphics card, you have an ideal machine to run ML workflows. There are many guides on installing Jupyter locally.

Otherwise, your best options are probably using the OS2G [HCC](hcc.unl.edu) usergroup, which is documented on the os2g webpage, or putting some money into running the workload on Amazon Web Services.

## Debugging
One of the primary challenges on using Tensorflow can be debugging the various errors you get. This is part of why it can be valuable to run your workload locally, as it becomes simpler to debug your issues. However, it is common to run into issues. Googling errors will solve the majority of issues you will encounter, but given how extensive Tensorflow is there's a good likelihood your exact bug won't be displayed. In these cases, your two best bets are the tensorflow documentation and finding people who have the skills to answer your questions.

### Tensorflow API Documentation
The Tensorflow API is incredibly well documented and can be found at https://www.tensorflow.org/versions. You can even use Tensorflow with Javascript if you're more comfortable with web programming. If you're calling a particular function, the structure of the API call will tell you which module a method is part of. Two great modules to get familiar with are [Keras](https://www.tensorflow.org/api_docs/python/tf/keras) and [IO](https://www.tensorflow.org/api_docs/python/tf/io).

### Communities

