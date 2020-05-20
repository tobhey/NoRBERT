## Get the artifacts
The artifacts can be downloaded from Zenodo: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3833661.svg)](https://doi.org/10.5281/zenodo.3833661) 

We provide a file containing all code, datasets and results (`NoRBERT_RE20_Paper65.zip`) as well as a file only containing the pretrained models (`NoRBERT_pretrained_models.zip`).

## How to use
To use the notebooks, we recommend you to load them into [Google Colab](https://colab.research.google.com/github/tobhey/NoRBERT).
Please make sure that you use a GPU (in Colab: Edit -> Notebook settings -> Hardware accelerator: GPU).

If you plan on running locally, you need to install [Jupyter](https://jupyter.org/install).
Furthermore, you might have to install further python dependencies than the ones installed in the notebooks (first cell) depending on your python installation.
You have to make sure that you installed all python libraries that are imported in the second cell via pip. 
You will need a machine with a very potent GPU (at least 12GB GPU RAM for the large models) as the pretrained BERT model is very memory hungry.

Each notebook has a cell with the configuration that can be adapted and allows tuning hyperparameters and configure experiment set-ups like sampling or folding strategy.
Details on the hyperparameters and settings are outlined in the respective [Notebooks](./Code/).

Make sure to correctly set paths to data folders/files as well as for logging output.
If using Google Colab, we recommend loading the data in your Google Drive, from where it can be imported.
Make sure to adapt the corresponding paths in the notebooks.
