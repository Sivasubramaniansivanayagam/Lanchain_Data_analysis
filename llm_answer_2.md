**Summary of Age Distribution in Each Department**

The age distribution of employees in each department is as follows:

* **Human Resources**: The average age is 37.81 years, with a standard deviation of 9.23 years. The age range is between 19 and 59 years, with 25% of employees being 30.5 years or younger, 50% being 37 years or younger, and 75% being 44 years or younger.
* **Research & Development**: The average age is 37.04 years, with a standard deviation of 9.18 years. The age range is between 18 and 60 years, with 25% of employees being 30 years or younger, 50% being 36 years or younger, and 75% being 43 years or younger.
* **Sales**: The average age is 36.54 years, with a standard deviation of 9.03 years. The age range is between 18 and 60 years, with 25% of employees being 30 years or younger, 50% being 35 years or younger, and 75% being 42 years or younger.

**Code Used**

```python
import pandas as pd

# Assuming df is your DataFrame
age_distribution = df.groupby('Department')['Age'].describe()

print(age_distribution)
```

**Result**

The result is a pandas DataFrame that provides a summary of the age distribution in each department, including the count, mean, standard deviation, minimum, 25th percentile, median (50th percentile), 75th percentile, and maximum age.

```
                         count       mean       std   min   25%   50%   75%  \
Department                                                                   
Human Resources          63.0  37.809524  9.226290  19.0  30.5  37.0  44.0   
Research & Development  961.0  37.042664  9.178964  18.0  30.0  36.0  43.0   
Sales                   446.0  36.542601  9.032611  18.0  30.0  35.0  42.0   

                         max  
Department                    
Human Resources         59.0  
Research & Development  60.0  
Sales                   60.0
```