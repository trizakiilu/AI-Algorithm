# AI-Algorithm
 My project
The project is in sections
First importing the libraries because we are creating a hierarichal clustering model to classify the wholesale dataset.
#Import moduels
#import pandas as pd
#import matplotlib.pyplot as plt
import numpy as np
import seaborn as sns
from matplotlib.ticker import PercentFormatter
Importing the datest in use
data = pd.read_csv('Wholesale customers data.csv')
data.head()
Plotting the hierarichal cluster
import scipy.cluster.hierarchy as shc
plt.figure(figsize=(10, 7))  
plt.title("Dendrograms")  
dend = shc.dendrogram(shc.linkage(data_scaled, method='complete'))