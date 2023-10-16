# Machine Learning Starter Kit

## Overview

Hello hackers, and welcome to the machine learning/deep learning starter kit! Feel free to clone this repository and play around with the notebooks. This quick starter kit will get you started with a brief overview of tools necessary to implement your own learning model. Namely, this guide will cover **conda environments, jupyter notebooks, and a quick overview of training your first PyTorch model.** 


### Why Machine Learning?
Why machine learning? _Well, the answer is both exciting and practical. Machine learning has become an integral part of our lives, shaping the way we interact with technology. From personalized recommendations on streaming platforms to self-driving cars and healthcare advancements, machine learning is at the heart of these innovations. It's not just for computer scientists and data wizards; it's a skill set that can empower anyone to solve complex problems, analyze data, and make informed decisions._ Recent technological innovations such as ChatGPT are the product of machine learning, capable of generating the entire italicized section above. 

### Goal and of the Starter Kit
Machine learning and deep learning is a very complex field. New models and architectures are constantly being developed and entire graduate level courses and seminars are devoted towards just grasping some of the math that goes on behind the scenes. That being said, with the help of some powerful democratized/open-sourced libraries such as PyTorch and TensorFlow, we can create our own models without worrying about all the finer details. Some models are also implemented for ready use in libraries such as `Scikit-learn`, but are not the focus of this starter kit.

### Starter Kit Structure

The starter kit is broken into 3 separate components. It is recommended to complete the steps in order. 

The [first step](1-conda.md) is to download and install Anaconda which will create a standalone environment with all the relevant dependencies/libraries (e.g. PyTorch). 

The [second step](2-jupyter.md) will get you familiar with running code in jupyter notebooks. Jupyter notebooks are useful given their easy accessibility and notebook/block formatting to run one code block at a time, but are also optional since notebooks or code blocks can also simply be run as scripts (though re-training a model each run might be a bit computationally heavy, so you would need a way to save the model).

The [third step](3-pytorch.ipynb) will lead you through the implementation of a simple machine learning model in PyTorch. Documentation and resources for further reading will be linked throughout the notebook for more details, but to avoid becoming a lecture on machine learning principles, the notebook will focus on syntax and a skeletal framework that can be easily used.