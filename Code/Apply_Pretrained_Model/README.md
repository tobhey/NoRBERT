# Apply pretrained NoRBERT models
The included notebooks enable to load a pretrained NoRBERT model and apply it to an input requirement.
Thus, one is able to try their abilities on any, probably unseen, input.

We provide models for Task 1 to 4 and the classification of functional requirement concerns.
Note that these models are trained on the whole respective dataset and therefore weren't used to produce any of the results.
We would love to provide the models we used to produce the results with, but as we used cross-validation this would result in a huge amount of model files. Considering the file size of each model this is not feasible.

Each model (.pkl) is accompanied by a .config file displaying the configuration used to train the model.

Pretrained model files can be found in [`NoRBERT_pretrained_models.zip`](https://doi.org/10.5281/zenodo.3833660) on Zenodo.

# How to use

The Notebooks are mostly self-explanatory. We also recommend to use Google Colab here. Elsewise some imported python libraries may have to be installed via pip.
One has to configure the path to the model file either locally or if using Colab via Google Drive connector.
