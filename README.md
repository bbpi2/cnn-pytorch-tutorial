# Image Recognition with Convolutional Neural Network Tutorial

👋👋👋 Welcome! This repo is a beginner friendly tutorial for building a Convolutional Neural Network (CNN) from scratch using PyTorch.

## 💳 Credit

<u>Introduction to Jupyter Notebooks & Python</u>

This was heavily borrowed and adapted from [this tutorial](https://github.com/ABS-Neural-Nets-Tutorial/Intro-To-Neural-Networks)

<u>Procedure of Building a CNN from PyTorch</u>

This tutorial was heavily borrowed from the [d2l.ia](http://d2l.ai/). Major changes made include:
* Simplification and adaptation to cpu-only implementation.
* Comments and descriptions of the functions.

Note the sample code in the d2l.ia [repo](https://github.com/d2l-ai/d2l-en) is subject to a modified [MIT License](https://en.wikipedia.org/wiki/MIT_License). 



## ✍️ How to Use

This will depend on whether or not you have had any experience with python and anaconda before.

<u>No Experience</u>

Simply click on the following link to open a [mybinder](https://mybinder.org/) application by clicking the button below:

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/bbpi2/cnn-pytorch-tutorial/HEAD?labpath=notebooks%2F0_Welcome.ipynb)

*Note: This may take several minutes to open.*

<u>Some Python/Anaconda Experience</u>

It is recommended that you clone this repo to your own device and then run the notebooks from there. You will have more access to resources than the mybinder application.

1. Install [Anaconda](https://docs.anaconda.com/anaconda/install/index.html) (Miniconda should also work, but Anaconda is recommended if you have the disc space)
2. Clone this repository to your local directory (either with `git clone` or just downloading the `.zip`)
3. Open 'Anaconda Prompt' from the start menu and create a new virtual environment `conda create -n cnn-tutorial`
4. Activate this new environment `conda activate cnn-tutorial`
5. Install `ipykernel` by running `conda install ipykernel`
6. Create a new Jupyter kernel and link by running `python -m ipykernel install --user --name=cnn-tutorial`. Note your anaconda prompt should have the `cnn-tutorial` environment active - eg:

```bash
(base) C:>
```
7. Install the key packages. There are two options:

Option A: Using Conda Environments:

* `cd` to `./binder` and run `conda env export --from-history -f environment.yml`

Option B: Manually Install Packages:

* Pytorch: `conda install pytorch torchvision torchaudio cpuonly -c pytorch`
* Matplotlib: `conda install matplotlib`

8. Open an instance of Jupyter Lab wherever you have clone this repo to (`cd` to the directory and run `jupyter lab`)
9. Set the kernel to be `cnn-tutorial` when running each notebook.

### Change Log

* Removed `torchaudio` and `cpuonly` since the `repo2docker` from binder cannot find these packages
