# PRODIGY_DS_Task1
#Data taken from oecd

#Create a bar chart or histogram to visualize the distribution of a categorical or continuous variable, such as the distribution of ages or genders in a population for given a dataset

import matplotlib.pyplot as plt
import pandas as pd
import numpy as np
df = pd.read_csv("/content/RPOP_09032024175622359.csv")
ages = np.random.randint(18, 80, size=1000)
plt.figure(figsize=(10, 7))
plt.hist(ages, bins=20, color='green', edgecolor='black')  # Adjust the number of bins as needed
plt.title('Distribution of Ages')
plt.xlabel('Age')
plt.ylabel('Frequency')
plt.show()
