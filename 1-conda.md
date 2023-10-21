# Conda Environments and Installation

## Overview
In order to set up your virtual environment, we _highly recommend_ (and only formally support) the use of Anaconda to create and manage your Python environment.


Virtual environments are tools that to keep dependencies required by different projects separate by creating isolated python virtual environments for them. This may be 
especially relevant if different versions of packages are required for 


1) Download [Anaconda](https://www.anaconda.com/download), and install it on your 
computer. You can alternatively download [Miniconda](https://docs.conda.io/projects/miniconda/en/latest/) if space is a concern. After running, restart your terminal.

> **Note:** If you have an existing Anaconda or Miniconda installation, then you don’t need to reinstall, and can just use that! To test if you have an existing conda installation, 
run `conda --version` in your terminal.

2) You can now set up your Conda environment [in a few ways](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html). A straight forward way is to run `conda create -n [your env name here]` (though Step 3 will have another installation method involving assistance in installing dependencies). 
After running this, you can run `conda env list` to confirm your list of environments. To delete an environment, run `conda env remove -n [your env name]`. From this point on, you can run `conda activate [your env name]`
to activate your environment. To deactivate it, run `conda deactivate`. 

3) Install necessary [dependencies](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-pkgs.html) (e.g. NumPy, PyTorch, etc.). Note that some niche packages may be in different channels, so if you cannot install them, you may need to [add them](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-channels.html). For any package that you need, run `conda install [package]` when in your environment. Some packages may have different syntaxes for installation (e.g. for PyTorch, you would run `conda install pytorch torchvision -c pytorch`), so make sure to view documentation when necessary. View all your current packages with `conda list`. 

You can also directly create an environment with packages installed using `yml` files. Create the environment instead with `conda env create -n [name_of_env] -f [path_to_yaml]`. A `yml` file has been provided for the following installation method.

> **Potential Issues**: If a `SpecNotFound` is raised: cd to the path where .yml is located, set [path_to_yaml] as your yml file. If your conda version is conda 4.12.0 or lower, and meet error on create environment, try running `conda env create -n [name_of_env] --file=[path_to_yaml]`.

You've now set up your first virtual environment! If you are familiar with jupyter notebooks, you can move directly to [the PyTorch guide](3-pytorch.ipynb). For a quick primer on notebooks, check out the [the jupyter guide](2-jupyter.md).
