[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3833660.svg)](https://doi.org/10.5281/zenodo.3833660)
![GitHub](https://img.shields.io/github/license/tobhey/NoRBERT)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tobhey/NoRBERT)

# NoRBERT: Transfer Learning for Requirements Classification
| :exclamation:  Please Note:  |
|-----------------------------------------|
|We found a bug in the notebooks that caused the indexing of the project-specific folds to be wrong. Thus, the results for the p-fold and loPo settings reported in the original paper are not correct as they were not strictly project-specific. We published a corrected Version of the paper at https://doi.org/10.5445/IR/1000150464. We fixed the bug in this version. The overall claim that NoRBERT performs better on unseen projects than existing approaches still holds true but the results on this type of folds are slighty worse (about 5 percentage points in F1-score on average) than reported.|

This is the supplementary material repository of the paper "NoRBERT: Transfer Learning for Requirements Classification".
In this paper we explore the performance of transfer learning (with Google's language model BERT) on different tasks in requirements classification. Especially the performance on projects, completely unseen during training, is in the focus of the paper.
Additionally, we developed a new dataset based on the Promise NFR dataset, that includes a more fine-grained labeling of functional requirement based on their concerns (Function, Data, Behavior).

This repository contains the datasets and code used in the paper, as well as additional results:

* [Dataset](./Dataset/) contains the labeled dataset for the classification of functional requirements concerns (based on Promise NFR dataset) as well as information about our labeling (results of each annotator and Krippendorf's Alpha, KALPHA)
* [Code](./Code/) contains the python notebooks (code) and datasets used for
	- [Task 1](./Code/Task1_to_3_original_Promise_NFR_dataset): Binary F/NFR classification (on Promise NFR dataset)
	- [Task 2](./Code/Task1_to_3_original_Promise_NFR_dataset): Classification of most frequent NFR subclasses (on Promise NFR dataset)
	- [Task 3](./Code/Task1_to_3_original_Promise_NFR_dataset): Classification of all NFR subclasses (on Promise NFR dataset)
	- [Task 4](./Code/Task4_relabeled_Promise_NFR_dataset): Functional and Quality aspects classification (on relabeled Promise NFR dataset)
	- [Task 5](./Code/Task5_func_concerns_dataset): Classification of functional requirement concerns (on functional concerns dataset)
	- [Notebooks](./Code/Apply_Pretrained_Model) to apply pretrained models for each task to an input requirement and pretrained models for each task
* [Results](./Results/) contains the results of all tested hyperparameter configurations for each task


| :exclamation:  Please Note:  |
|-----------------------------------------|
|Note that we calculated the overall results of the cross validations by collecting the predictions of all folds and calculating the metrics over all predictions instead of averaging the results per metric over the folds. However, our notebooks provide both results. |

| :exclamation:  Please Note:  |
|-----------------------------------------|
|Note that we are not able to provide the actual models that were used to produce the results of the paper. We used cross validation experiments that would result in a huge amount of model files per experiment run on each task. As the model files are quite large this is not feasible. The results may still be reproduced with the supplied notebooks.|

## Attribution (of datasets used)
The Promise Dataset can be attributed to Jane Cleland-Huang and was provided for the RE'17 Data Challenge.<br>
Jane Cleland-Huang, Sepideh Mazrouee, Huang Liguo, & Dan Port. (2007). nfr [Data set]. Zenodo. Available: http://doi.org/10.5281/zenodo.268542<br>
RE'17 Data Challenge: http://ctp.di.fct.unl.pt/RE2017/pages/submission/data_papers/<br>
See also:
Sayyad Shirabad, J. and Menzies, T.J. (2005) The PROMISE Repository of Software Engineering Databases. School of Information Technology and Engineering, University of Ottawa, Canada. Available: http://promise.site.uottawa.ca/SERepository

The relabeled Promise dataset can be attributed to Dalpiaz et al.:
F. Dalpiaz, D. Dell’Anna,  F. B. Aydemir, and  S. Çevikol, “explainable-re/re-2019-materials,” Jul.2019. https://doi.org/10.5281/zenodo.3309669
