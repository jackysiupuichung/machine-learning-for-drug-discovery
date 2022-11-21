# machine-learning-for-drug-discovery

## topic 1: Identifying targets for cancer using gene expression profiles 

### goal: 
accelerate drug discovery by identifying potential cancer related gene targets using machine learning approaches

### method:
- xgboost decision tree for multi-class classification
  - wrapped in sklearn MultiOutputClassifier
- prelimianry data augmentation
  - pca to lower dimensionality
  - normalize gene expression values
- model feeding
  - iterative stratification, weight adjustment for imbalanced dataset
- result interpretation
  - feature selection based on model's feature importance => check for gene from pca reduction

### data:
part of the RNA-Seq (HiSeq) PANCAN data set, it is a random extraction of gene expressions of patients having different types of tumor: BRCA, KIRC, COAD, LUAD and PRAD. (Weinstein, John N., et al. 'The cancer genome atlas pan-cancer analysis project.' Nature genetics 45.10 (2013): 1113-1120.)

