# classification
## table of contents
-[Importing Libraries](import-libraries)
-[Loading and Preparing the Iris Dataset](loading-and-preparing-datasets)

 Importing Libraries:
 ```bash
import matplotlib.pyplot as plt
from sklearn import datasets
from sklearn.cluster import KMeans
import sklearn.metrics as sm
import pandas as pd
import numpy as np
```
This section imports the necessary libraries:
1. matplotlib.pyplot: Used for creating visualizations.
2. datasets from sklearn: Provides access to the Iris dataset.
3. KMeans from sklearn.cluster: Implements the K-Means clustering algorithm.
4.sm from sklearn.metrics: Includes functions for evaluating model performance.
5. pandas and numpy: Used for data manipulation.

 
 Loading and Preparing the Iris Dataset:
```bash
iris = datasets.load_iris()

X = pd.DataFrame(iris.data)
X.columns = ['Sepal_Length','Sepal_Width','Petal_Length','Petal_Width']

y = pd.DataFrame(iris.target)
y.columns = ['Targets']
```
