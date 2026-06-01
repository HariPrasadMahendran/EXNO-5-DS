# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
 ```
import matplotlib.pyplot as plt
import pandas as pd
from sklearn.datasets import load_iris

# STEP 1: Load dataset
iris = load_iris()

# STEP 2: Convert to DataFrame
df = pd.DataFrame(
   iris.data,
   columns=iris.feature_names
)
```
```
# STEP 3: Visualize data

# Line Plot
plt.figure(figsize=(6,4))
plt.plot(df["sepal length (cm)"])
plt.title("Line Plot")
plt.xlabel("Index")
plt.ylabel("Sepal Length")
plt.show()
```
<img width="694" height="394" alt="image" src="https://github.com/user-attachments/assets/f83d425a-8468-48aa-bf77-78f81ff87549" />
```
# Histogram
plt.figure(figsize=(6,4))
plt.hist(df["petal length (cm)"], bins=10)
plt.title("Histogram")
plt.xlabel("Petal Length")
plt.ylabel("Frequency")
plt.show()
```
<img width="605" height="392" alt="image" src="https://github.com/user-attachments/assets/6dbab17f-b91b-4c43-80a0-1a0c310d8c91" />
```

# Scatter Plot
plt.figure(figsize=(6,4))
plt.scatter(
    df["sepal length (cm)"],
    df["petal length (cm)"]
)
plt.title("Scatter Plot")
plt.xlabel("Sepal Length")
plt.ylabel("Petal Length")
plt.show()

```
<img width="543" height="393" alt="image" src="https://github.com/user-attachments/assets/11ae6eea-7425-4a05-803a-50debf49bf0a" />
```

# Bar Plot
plt.figure(figsize=(6,4))
df.mean().plot(kind="bar")
plt.title("Average Feature Values")
plt.ylabel("Value")
plt.show()

```
<img width="573" height="483" alt="image" src="https://github.com/user-attachments/assets/88fb3347-14f2-4234-8d1a-687e87dbe637" />
```

# Box Plot
plt.figure(figsize=(6,4))
plt.boxplot(df["sepal width (cm)"])
plt.title("Box Plot")
plt.show()
```
<img width="534" height="376" alt="image" src="https://github.com/user-attachments/assets/edd88b19-2265-4a15-ab7f-67396d2d3e48" />


# Result:
 Include your result here
