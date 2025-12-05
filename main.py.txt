import pandas as pd
import numpy as np
from scipy import stats
from statsmodels.stats.weightstats import ztest

# Load data
df = pd.read_csv("StudentsPerformance.csv")

# Example columns
math = df['math score']
reading = df['reading score']

# --------------------- T-TEST ---------------------
t_stat, t_p = stats.ttest_ind(math, reading)
print("T-test: statistic =", t_stat, "p-value =", t_p)

# --------------------- Z-TEST ---------------------
z_stat, z_p = ztest(math, reading)
print("Z-test: statistic =", z_stat, "p-value =", z_p)

# --------------------- F-TEST ---------------------
var1 = np.var(math)
var2 = np.var(reading)
f_stat = var1 / var2
print("F-test: statistic =", f_stat)
