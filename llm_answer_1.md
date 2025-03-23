**Summary of Education Field and Department of Employees**

The provided dataframe contains information about 1470 employees, including their education field and department. The unique education fields are:

* Social Sciences
* Other
* Health Science
* Business
* Engineering
* Human Resources

The unique departments are:

* Sales
* Research & Development
* Human Resources

**Count of Each Education Field and Department**

The count of each education field is:

* Social Sciences: 606
* Health Science: 464
* Business: 159
* Engineering: 132
* Other: 82
* Human Resources: 27

The count of each department is:

* Research & Development: 961
* Sales: 446
* Human Resources: 63

**Education Field and Department for Each Employee**

The dataframe contains the education field and department for each employee.

**Count of Each Education Field in Each Department**

The count of each education field in each department is:

* Human Resources:
	+ Human Resources: 27
	+ Social Sciences: 16
	+ Health Science: 13
	+ Engineering: 4
	+ Other: 3
* Research & Development:
	+ Social Sciences: 440
	+ Health Science: 363
	+ Engineering: 94
	+ Other: 64
* Sales:
	+ Business: 159
	+ Social Sciences: 150
	+ Health Science: 88
	+ Engineering: 34
	+ Other: 15

**Count of Each Department in Each Education Field**

The count of each department in each education field is:

* Business:
	+ Sales: 159
* Engineering:
	+ Research & Development: 94
	+ Sales: 34
	+ Human Resources: 4
* Health Science:
	+ Research & Development: 363
	+ Sales: 88
	+ Human Resources: 13
* Human Resources:
	+ Human Resources: 27
* Other:
	+ Research & Development: 64
	+ Sales: 15
	+ Human Resources: 3
* Social Sciences:
	+ Research & Development: 440
	+ Sales: 150
	+ Human Resources: 16

**Code Used**

The code used to generate these results is:
```python
# Get unique EducationField and Department
print("Unique EducationField: ", df['EducationField'].unique())
print("Unique Department: ", df['Department'].unique())

# Get count of each EducationField and Department
print("Count of each EducationField: ", df['EducationField'].value_counts())
print("Count of each Department: ", df['Department'].value_counts())

# Get EducationField and Department for each employee
print("EducationField and Department for each employee: ")
print(df[['EducationField', 'Department']])

# Get count of each EducationField in each Department
print("Count of each EducationField in each Department: ")
print(df.groupby('Department')['EducationField'].value_counts())

# Get count of each Department in each EducationField
print("Count of each Department in each EducationField: ")
print(df.groupby('EducationField')['Department'].value_counts())
```
**System Code**

The system code used to execute this code is Python, specifically the pandas library for data manipulation and analysis. The code is executed in a Jupyter Notebook or a similar environment.