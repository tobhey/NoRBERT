## How to use
To use the notebooks, we recommend you to load them into [Google Colab](https://colab.research.google.com/github/tobhey/NoRBERT).
Please make sure that you use a GPU (in Colab: Edit -> Notebook settings -> Hardware accelerator: GPU).

If you plan on running locally, you need to install [Jupyter](https://jupyter.org/install).
Furthermore you might have to install further python dependencies then the ones installed in the notebooks (first cell), depending on your python installation.
You have to make sure that you installed all python libraries that are imported in cell2 via pip. 
You will need a machine with a very potent GPU (at least 12GB GPU RAM) as the pretrained BERT model is memory hungry.

Each notebook has a cell with the configuration that can be adapted and allows to tune hyperparameters and configure experiment set ups like sampling or folding strategy.
Details on the hyperparameters and settings are outlined in the respective [Notebooks](./Code/).

Make sure to correctly set paths to data folders/files as well as for logging output.
If using Google Colab, we recommend to load the data in your Google Drive, from where it can be imported.
Make sure to adapt the corresponding paths in the notebooks.