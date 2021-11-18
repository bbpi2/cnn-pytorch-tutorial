# CNN `PyTorch` Tutorial
 Basic tutorial for building CNN from scratch in PyTorch.

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/bbpi2/cnn-pytorch-tutorial/dev)


### Running in your own environment

1. Install [Anaconda](https://docs.anaconda.com/anaconda/install/index.html) (Miniconda should also work, but Anaconda is recommended if you have the disc space)
2. Clone this repository to your local directory
3. Open 'Anaconda Prompt' from the start menu and create a new virtual environment `conda create -n cnn-tutorial`
4. Activate this new environment `conda activate cnn-tutorial`
5. Install `ipykernel` by running `conda install ipykernel`
6. Link the conda environment to a Jupyter kernel by running `python -m ipykernel install --user --name=cnn-tutorial` (note the conda environment `cnn-tutorial` must be activated -- check if `(cnn-tutorial)` shows at the start of you anaconda prompt). At this point your conda environment and jupyter kernel should be linked. When you `conda install` a new package, you only need to restart your jupyter kernel for the changes to take place.
7. Install CPU-only version of pytorch`conda install pytorch torchvision torchaudio cpuonly -c pytorch`
8. Install matplotlib `conda install matplotlib`
9. Open a new instance of jupyter notebook from the local directory and set the kernel to be `cnn-tutorial`

NOTE: Steps 7-8 can be skipped if we just pulled from the `environment.yml` file (generated using `conda env export --from-history -f environment.yml`)



### Change Log

* Removed `torchaudio` and `cpuonly` since the `repo2docker` from binder cannot find these packages

*this is a branch*

