# learning-data-science
record about my data science learning
import re
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

import warnings
warnings.filterwarnings('ignore')

%matplotlib inline
train_data = pd.read_csv('data/train.csv')
test_data = pd.read_csv('data/test.csv')

sns.set_style('whitegrid')
train_data.head()
train_data.info()
print("-" * 40)
test_data.info()
train_data['Survived'].value_counts().plot.pie(autopct = '%1.2f%%')

