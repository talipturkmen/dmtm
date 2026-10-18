# dmtm: data mining course notebooks

> **Archived.** This is a 2020 course/learning project and is no longer maintained.

A collection of Jupyter notebooks written while working through a data mining and machine learning course. Each folder contains one topic, with the notebook(s) and the datasets they use. The notebooks are mostly tutorial-style: they load a dataset, explore it, apply one or more methods, and plot or print the results. No results are presented here beyond what the notebooks themselves show.

## Contents

| Topic | Folder | Notebook(s) | What it covers |
|---|---|---|---|
| Data exploration | `DataExploration-Iris/` | `DataExplorationIris.ipynb` | Basic exploration and statistics of the Iris dataset |
| Data exploration | `DataExploration-HousePrices/` | `HousePricesPart1.ipynb` | Exploration of the Kaggle house prices data, missing values, linear regression |
| Anscombe's quartet | `Anscombes+Quartet/` | `AnscombesQuartet.ipynb` | Why summary statistics alone are not enough to describe a dataset |
| Regression | `LinearRegression.ipynb/` | `LinearRegression.ipynb` | Linear regression and polynomial regression on Boston housing data |
| Regression | `GeneratingPolynomialFeatures.ipynb/` | `GeneratingPolynomialFeatures.ipynb` | Generating polynomial features with scikit-learn |
| Regression | `RidgeAndLassoRegression.ipynb/` | `RidgeAndLassoRegression.ipynb` | Linear, ridge and lasso regression on a small generated dataset |
| Regression | `kNNRegression/` | `kNNRegression.ipynb` | k-nearest neighbors regression |
| Regression | `AnalysisOfTheBostonHousingDataset/` | `AnalysisOfTheBostonHousingDataset.ipynb` | Regression analysis of the Boston housing dataset |
| Classification | `LogisticRegressionMulticlass/` | `Logistic Regression Multiclass Iris.ipynb` | Multiclass logistic regression on Iris |
| Classification | `LogisticRegressionOverfitting/` | `LogisticRegressionOverfittingExample.ipynb` | Overfitting in classification with logistic regression |
| Classification | `Loan+Prediction/` | `Loans-Safety-Prediction.ipynb` | Predicting whether a loan is safe to assign; compares several models (see `LoanSafety-Summary*.csv`). Includes a PDF report |
| Clustering | `kMeans/` | `kMeans Animated Examples.ipynb`, `kMeansClustering.ipynb`, `kMeans-Assumptions-WithCentroids.ipynb` | k-means, animated example, elbow analysis, and cases where k-means assumptions fail |
| Clustering | `Hierarchical+Clustering/` | `HierarchicalClustering.ipynb`, `ClusteringValidation-*.ipynb` | Hierarchical clustering and external/internal validation measures on Iris |
| Clustering | `SilhouetteAnalysis/` | `SilhouetteAnalysis.ipynb`, `SilhouetteAnalysisIris.ipynb` | Silhouette analysis for k-means |
| Clustering | `Clustering+Comparison/` | `ComparisonOfClusteringMethods.ipynb` | Comparison of clustering algorithms on toy datasets |
| Feature selection | `Feature+Selection/` | `FeatureSelectionMethods.ipynb` | Feature selection methods compared against a baseline |
| Resampling | `Bootstrap/` | `Bootstrap.ipynb`, `BootstrapeResamplingEvaluation.ipynb` | Bootstrap resampling, and bootstrap-based classifier evaluation |
| Association rules | `Association+Rule+Mining/` | `Association Rules Examples.ipynb`, `PrintSequence.py` | Association rule mining (R `arules` example) and SPMF sample datasets in `test_files/` |
| Time series | `Data+Series/` | `DataSeries-Part1-Basics.ipynb`, `-Part2-Modeling.ipynb`, `-Part3-Evaluation.ipynb` | Time series basics, modeling and evaluation. Data in `stocks/`, `co2/`, `others/` |
| Time series | `AnalysisOfFREDData/` | `AnalysisOfFREDData.ipynb` | Predicting real personal consumption expenditures from FRED data (`fred_data.csv`) |

`Data+Series/Data Series/others/Untitled.ipynb` is an empty notebook and is kept as it was.

## Tech stack

- Python 3, Jupyter Notebook (kernel `python3` in all notebooks)
- pandas, NumPy, SciPy, scikit-learn, matplotlib, seaborn, statsmodels, pmdarima (as imported by the notebooks)
- The association rules notebook calls the R `arules` package (`library(arules)`).

## Running

1. Install Python 3 and Jupyter, plus the libraries listed above (no requirements file was kept).
2. Start Jupyter from the repository root or from a topic folder:

   ```
   jupyter notebook
   ```

3. Open a notebook and run it. Paths in the notebooks are relative to their own folder, so run each notebook from its own directory.

The notebooks were not re-run as part of the archiving cleanup. Some may depend on package versions from 2020 and may need small changes to run with current libraries.

## Notes

- Build artifacts from the original macOS zip exports (`.ipynb_checkpoints/`, `__MACOSX/`, `.DS_Store`) were removed from the repository. The notebooks themselves are unchanged.
