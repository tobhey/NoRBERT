## Get the artifacts
The artifacts can be downloaded from Zenodo: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3833660.svg)](https://doi.org/10.5281/zenodo.3833660)

We provide a file containing all code, datasets and results (`NoRBERT_RE20_Paper65.zip`) as well as a file only containing the pretrained models (`NoRBERT_pretrained_models.zip`).

## How to use
To use the notebooks, we recommend you to load them into [Google Colab](https://colab.research.google.com/github/tobhey/NoRBERT) (this link opens the submission repository directly in Colab and allows you to open one of the notebooks).
With Colab, you should be able to open the notebooks, set the preferred configuration parameters and run all cells (CTRL+F9 or Runtime -> Run All).
A GPU as hardware accelerator should already be used by Colab.
We have a cell that checks if a GPU is used; if it turns out that none is used, please enable the GPU (in Colab: Edit -> Notebook settings -> Hardware accelerator: GPU).

If you plan on running locally, you need to install [Jupyter](https://jupyter.org/install).
Furthermore, you might have to install further python dependencies than the ones installed in the notebooks (first cell) depending on your python installation.
You have to make sure that you installed all python libraries that are imported in the second cell via pip.
It is neccessary to install [PyTorch](https://pytorch.org/get-started/locally/#start-locally).
You will need a machine with a very potent GPU (at least 12GB GPU RAM for the large models) as the pretrained BERT model is very memory hungry.
Also, you have to make sure that your GPU and drivers support CUDA.
We recommend Ubuntu as operating system.
Moreover, some parts of the notebooks are coded and designed for Colab; there might be some differences in appearance.
There should be no problems regarding the code, but there is still the possibility that you might experience some issues (regarding your installation, system, setup etc.).

Each notebook has a cell with the configuration that can be adapted and allows tuning hyperparameters and configure experiment set-ups like sampling or folding strategy.
Details on the hyperparameters and settings are outlined in the respective [Notebooks](./Code/).

Make sure to correctly set paths to data folders/files as well as for logging output.
If using Google Colab, you have two options (can be set in the configuration cell):
1. Loading the data from zenodo. This downloads the zip from zenodo using wget and extracts the needed data set. The log will be stored in the working directory. You can access everything in Colab by browsing to the "Files" tab on the left.
2. Loading the data in your Google Drive, from where it can be imported. Logs will also be stored on your Google Drive.
Make sure to update the corresponding paths in the notebooks to your needs.
