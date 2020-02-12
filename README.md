# NoRBERT: Transfer Learning for Requirements Classification
This is the repository for the paper "NoRBERT: Transfer Learning for Requirements Classification".

This repository contains code and datasets used in the paper:
* [Promise](./Promise/) contains the python notebooks (code) for Task1 (F/NFR binary class.), Task2 (most frequent NFR subclasses class. of), and Task3 (all NFR subclasses class.). Also contains the used dataset.
* [Promise_relabeled](./Promise_relabeled/) contains the relabeled PROMISE dataset along with our python notebooks (code). This represents Task4.
* [func_nfr](./func_nfr/) contains the labeled dataset, information about our labeling (including Krippendorf's Alpha, KALPHA), and our python notebooks.

## How to use
To use the notebooks, we recommend you to load them into [Google Colab](colab.research.google.com/).
In each notebook is a cell with the configuration that can be tuned.
Make sure to correctly set paths to data folders/files as well as for logging output.
We recommend you to load the data in your Google Drive, from where it can be imported.
Make sure to adapt the corresponding paths in the notebooks.