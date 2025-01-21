df.to_csv('chronic_kidney_disease.csv', index=False) was used to transform to csv.

EXAMPLE

from ucimlrepo import fetch_ucirepo 
import pandas as pd
# fetch dataset 
breast_cancer_wisconsin_diagnostic = fetch_ucirepo(id=17) 
  
# data (as pandas dataframes) 
X = breast_cancer_wisconsin_diagnostic.data.features 
y = breast_cancer_wisconsin_diagnostic.data.targets 
  
df = pd.concat([X, y], axis=1)
#%%
df.to_csv('knn_cancer_wisconsin.csv', index=False)