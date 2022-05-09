# cs-598-dlh-paper-32

# Dependencies
* Python >= 3.8.11
* Please use conda to install all the dependencies using the command
  * `conda env create -f environment.yml`

# How to run the code
Once you install the dependency, please run the following code to open Jupyter Notebook on your terminal (Mac OS/Linux system)
* `jupyter notebook`

# Data download instruction
The filtered data of MIMIC-III is `dataset/t1` folder. We only use a subset of MIMIC-III and it is filtered based on the requirement in the paper. This subset of MIMIC-III is already decoded that does not contains any original information from the original MIMIC-III.

The file 'Extract MIMIC III Dataset.ipynb` contains code to extract patient information from the raw MIMIC III Dataset.

# Table of results
## Macro-Averging Measures of Disease Prediction
| Method  |  Accuracy |  Recall | Precision  |  F1 Score |
|---|---|---|---|---|
|  Euclidean |  0.3703 |  0.38209 |  0.4264 |  0.2907 |
| Cosine  |  0.3925 |  0.4061 | 0.3968  |  0.3842 |
|  CNN-triple |  0.4888 |  0.4832 |  0.4832 |  0.4824 |

## Patient Clustering Performance Based on Learned Distance
| Method  |  Rand index |  Purity |  NMI |
|---|---|---|---|
|  Euclidean |  0.4284 |  0.4 |  0.0190 |
|  Cosine |  0.5473 |  0.4074 |  0.0162 |
|  CNN-triplet | 0.5653  |  0.4888 |  0.0679 |

# Citation:
1. Suo, Q., Ma, F., Yuan, Y., Huai, M., Zhong, W., Gao, J., Zhang, A. (2018). Deep Patient Similarity Learning for Personalized Healthcare. IEEE transac- tions on nanobioscience, 17(3), 219–227. https://doi.org/10.1109/TNB.2018.2837622
