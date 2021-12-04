# Parkinson disease prediction using feature selection technique in machine learning

by
Author 1: Tamim Wasif,
Author 2: Md. Inzamam Ul Hossain,
Author 3: Asif Mahmud



> This is a paper of the disease Parkinson, which is a human disease. Here we worked with the Parkinson's UCI Machine Learning Repository dataset. We have researched with the dataset. We researched if there is any error in the dataset or not. We used some famous machine learning (ML) algorithms and methods so that we can get the highest accuracy, and we got the accuracy of 97.43%

| **Classifier**|**Accuracy(%)**| **Medhod**    | **Features Used** |**Sensitivity**|**Specificity**| **AUC**       |
| ------------- | ------------- | ------------- | -------------     | ------------- | ------------- | ------------- |
| XGBoost       |  **97.43**    | RFE           | 9                 | 1.0           | 85.71         |  92.85        |
| KNN           |  **97.43**    | UncorrelatedF-| 11                | 96.8          | 1.0           |  98.43        |
| Random Forest | 94.87         | UncorrelatedF-| 11                | 1.0           | 71.42         |  85.71        |
| SVM           | 92.30         | RFE           | 12                | 1.0           | 57.14         | 78.57         |
| Neural Network| 87.18         | RFE(XGBoost)  | 22                | -             | -             | -             |

This paper has been submitted for publication in IEEE in the conference of Kharagpur, India.


## Abstract

> Parkinson's is a complex disease. That includes
numerous physical, mental, and neurological assessments. The 
Assessments incorporate examining various signs and side 
effects, exploring the clinical history, and checking the sensory 
system states. In our proposed method, we applied five different 
classifiers. This paper aims to increase the accuracy and 
optimize the feature used in the dataset. We used the hybrid 
feature selection method for optimization, which combines the 
wrapper and filter methods. The method name is Recursive 
Feature Elimination. The highest accuracy was gained by the 
classifier XGBoost, 97.43%, with nine features out of 22 
features.


## Software implementation

> We used Jupyter Notebook for python and anaconda prompt. [Jupyter notebooks](http://jupyter.org/).

You will get all the code files in the repository.


## Getting the code

You can download a copy of all the files in this repository by cloning the
[git](https://git-scm.com/) repository:

    git clone https://github.com/tamimjdd/Thesis-final.git

or [download a zip archive](https://github.com/pinga-lab/PAPER-REPO/archive/master.zip).

A copy of the repository is also archived at 10.1109/ICCCNT51525.2021.9580151


## Dependencies

You'll need a working Python environment to run the code.
The recommended way to set up your environment is through the
[Anaconda Python distribution](https://www.anaconda.com/download/) which
provides the `conda` package manager.
Anaconda can be installed in your user directory and does not interfere with
the system Python installation.
The required dependencies are specified in the file `environment.yml`.

We use `conda` virtual environments to manage the project dependencies in
isolation.
Thus, you can install our dependencies without causing conflicts with your
setup (even with different Python versions).

Run the following command in the repository folder (where `environment.yml`
is located) to create a separate environment and install all required
dependencies in it:

    conda env create


## Reproducing the results

Before running any code you must activate the conda environment:

    source activate ENVIRONMENT_NAME

or, if you're on Windows:

    activate ENVIRONMENT_NAME

This will enable the environment for your current terminal session.
Any subsequent commands will use software that is installed in the environment.

To build and test the software, produce all results and figures, and compile
the manuscript PDF, run this in the top level of the repository:

    make all

If all goes well, the manuscript PDF will be placed in `manuscript/output`.

You can also run individual steps in the process using the `Makefile`s from the
`code` and `manuscript` folders. See the respective `README.md` files for
instructions.

Another way of exploring the code results is to execute the Jupyter notebooks
individually.
To do this, you must first start the notebook server by going into the
repository top level and running:

    jupyter notebook

This will start the server and open your default web browser to the Jupyter
interface. In the page, go into the `code/notebooks` folder and select the
notebook that you wish to view/run.

The notebook is divided into cells (some have text while other have code).
Each cell can be executed using `Shift + Enter`.
Executing text cells does nothing and executing code cells runs the code
and produces it's output.
To execute the whole notebook, run all cells in order.


## License
The manuscript text is not open source. The authors reserve the rights to the
article content, which is currently submitted for publication in the
IEEE.
