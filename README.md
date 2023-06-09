# DLH Reproducibility Project Multi-Modality Machine Learning Predicting Parkinson’s Disease

## Summary
Early and accurate detection of Parkinson's disease (PD), before an individual suffers from any symptoms, is essential for effective intervention. The researchers of the paper [Multi-modality machine learning predicting Parkinson’s disease](https://www.nature.com/articles/s41531-022-00288-w#data-availability) aim at combining machine learning and multi-modal data, to develop better predictive models, and thus contribute to early and correct diagnosis and identification of (potential) high-risk individuals. In addition, the goal of the researchers is to build models based on remotely attainable data, and do not require additional clinic visits to a specialist.

The researchers leveraged an automated ML open-source Python package, GenoML, to carry out the analysis. This package automatically compares the best performing machine learning algorithms.

The goal of our study is to reproduce the research, and test whether the claims of the paper are accurate. For our study we heavily relied on the code of the original paper, and likewise used GenoML. We used data from AMP PD. As this data may not be published publicly, we cannot add the data to this repository.


## Helpful Links 
- [Source code original research paper](https://github.com/GenoML/GenoML_multimodal_PD/)
- [GenoML short paper](http://arxiv.org/abs/2103.03221v1)
    - [GenoML website](https://genoml.com/)
    - [GenoML repository](https://github.com/GenoML/genoml2)
- [AMP PD](https://amp-pd.org/)


## Requirements
In order to use GenoML, you will need to `pip install genoml2` or `git clone https://github.com/GenoML/genoml2.git`. Furthermore a Python version of 3.5 or higher is required and 'R' needs to be installed. Moreover, the requirements of GenoML (as listed in their requirements.txt) need to be installed, which can be done in a virtual environment. In order to check whether the installation of GenoML has worked, their website provided several example files and code that can be run. These examples can be run from the command line.

GenoML suggests working on linux or mac for the best results.


## Orientation 
- The `ReproducibilityStudy.ipynb` file contains our code for the reproducibility study. This is still work in progress as we await access to tier 2 data. 
- The `SummaryofReproducibilityStudy.ipynb` file will summarize our reproducibility study when our project is finished. Hence, this file only consists of a template, but does not contain any content yet.
- The `DataModels.ipynb` file contains details of the models of the original research paper by reading in the joblib files of the 49 models contained in the repository of the researchers. Considering we do not yet have access to the tier 2 data, it was not possible to reproduce the research paper. However, reading in these joblib files gave us some insights. 
- The `data` folder contains the placeholder data. Once we obtain full access to tier 2 data, we cannot publish this publicly. So the data folder will never contain actual Parkinson's data. However, since we do not have access to the tier 2 data yet, we temporarily created placeholder data, for our code to run with some input.
- The `outputs` folder contains the output files after running the GenoML code. This is empty, as our data and results cannot be published publicly, however, to prevent and IO failure when running the code after cloning, the folder is added to the repository.
- The `original_trained` folder contains joblib files with several models of the original paper (as uploaded in their repository). We use these files in `DataModels.ipynb` to get a better understanding of the original models.
- - The `original_tuned` folder contains joblib files with several models of the original paper (as uploaded in their repository). We use these files in `DataModels.ipynb` to get a better understanding of the original models.
