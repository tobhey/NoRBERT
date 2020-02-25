# NoRBERT: Transfer Learning for Requirements Classification
This is the repository for the paper "NoRBERT: Transfer Learning for Requirements Classification".

This repository contains code and datasets used in the paper:
* [Promise](./Promise/) contains the python notebooks (code) for Task1 (F/NFR binary class.), Task2 (most frequent NFR subclasses class. of), and Task3 (all NFR subclasses class.). Also contains the used dataset.
* [Promise_relabeled](./Promise_relabeled/) contains the relabeled PROMISE dataset along with our python notebooks (code). This represents Task4.
* [func_nfr](./func_nfr/) contains the labeled dataset for the classification of functional requirements, information about our labeling (including Krippendorf's Alpha, KALPHA), and our python notebooks.
* NoRBERT_use.ipynp allows to load a pretrained model and experiment with different inputs. Note: Currently, we cannot offer pretrained models, yet

## How to use
To use the notebooks, we recommend you to load them into [Google Colab](https://colab.research.google.com/github/norbert-one/NoRBERT).
Please make sure that you use a GPU (in Colab: Edit -> Notebook settings -> Hardware accelerator: GPU).

In each notebook is a cell with the configuration that can be tuned.
Make sure to correctly set paths to data folders/files as well as for logging output.
We recommend you to load the data in your Google Drive, from where it can be imported.
Make sure to adapt the corresponding paths in the notebooks.


## Attribution
The Promise Dataset can be attributed to Jane Cleland-Huang and was provided for the RE'17 Data Challenge.<br>
Jane Cleland-Huang, Sepideh Mazrouee, Huang Liguo, & Dan Port. (2007). nfr [Data set]. Zenodo. Available: http://doi.org/10.5281/zenodo.268542<br>
RE'17 Data Challenge: http://ctp.di.fct.unl.pt/RE2017/pages/submission/data_papers/<br>
See also: 
Sayyad Shirabad, J. and Menzies, T.J. (2005) The PROMISE Repository of Software Engineering Databases. School of Information Technology and Engineering, University of Ottawa, Canada . Available: http://promise.site.uottawa.ca/SERepository 

The relabeled dataset can be attributed to Dalpiaz et al:
F. Dalpiaz, D. Dell’Anna,  F. B. Aydemir, and  S. Çevikol, “explainable-re/re-2019-materials,” Jul.2019. https://doi.org/10.5281/zenodo.3309669
