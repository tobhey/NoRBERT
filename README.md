# NoRBERT: Transfer Learning for Requirements Classification
This is the supplementary material repository of the paper "NoRBERT: Transfer Learning for Requirements Classification".

This repository contains datasets and code used in the paper plus additional results:

* [Dataset](./Dataset/) contains the labeled dataset for the classification of functional requirements concerns (based on Promise NFR dataset) as well as information about our labeling (results of each annotator and Krippendorf's Alpha, KALPHA)
* [Code](./Code/) contains the python notebooks (code) and used datasets for 
	- [Task 1](./Code/Task1_to_3_original_Promise_NFR_dataset): Binary F/NFR classification (on Promise NFR dataset)
	- [Task 2](./Code/Task1_to_3_original_Promise_NFR_dataset): Classification of most frequent NFR subclasses (on Promise NFR dataset)
	- [Task 3](./Code/Task1_to_3_original_Promise_NFR_dataset): Classification of all NFR subclasses (on Promise NFR dataset)
	- [Task 4](./Code/Task4_relabeled_Promise_NFR_dataset): Functional and Quality aspects classification (on relabeled Promise NFR dataset)
	- [Task 5](./Code/Task5_func_concerns_dataset): Classification of functional requirements concerns (on functional concerns dataset)
	- [Notebook](./Code/Apply_Pretrained_Model) to apply pretrained models to Task 5
* [Results](./Results/) contains the results of all tested hyperparameter configurations for each task

## Attribution
The Promise Dataset can be attributed to Jane Cleland-Huang and was provided for the RE'17 Data Challenge.<br>
Jane Cleland-Huang, Sepideh Mazrouee, Huang Liguo, & Dan Port. (2007). nfr [Data set]. Zenodo. Available: http://doi.org/10.5281/zenodo.268542<br>
RE'17 Data Challenge: http://ctp.di.fct.unl.pt/RE2017/pages/submission/data_papers/<br>
See also: 
Sayyad Shirabad, J. and Menzies, T.J. (2005) The PROMISE Repository of Software Engineering Databases. School of Information Technology and Engineering, University of Ottawa, Canada . Available: http://promise.site.uottawa.ca/SERepository 

The relabeled dataset can be attributed to Dalpiaz et al:
F. Dalpiaz, D. Dell’Anna,  F. B. Aydemir, and  S. Çevikol, “explainable-re/re-2019-materials,” Jul.2019. https://doi.org/10.5281/zenodo.3309669
