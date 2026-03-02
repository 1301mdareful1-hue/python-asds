# Attributes & Methods Reference - All Lectures

---

# Lec 1: Python Basics

## File 1: Lec-1-lab-1.ipynb

### Python Built-in Methods (Lists & Dictionaries)
| Method | Type | Description |
|--------|------|-------------|
| `.append()` | List | Add element to end of list |
| `.remove()` | List | Remove first occurrence of element |
| `.pop()` | List | Remove and return element |
| `.keys()` | Dictionary | Return all dictionary keys |
| `type()` | Function | Return data type of object |
| `len()` | Function | Return length of sequence |
| `range()` | Function | Generate sequence of numbers |
| `sum()` | Function | Sum all elements |

## File 2: lec-1-practices.ipynb

### Python Built-in Methods
| Method | Type | Description |
|--------|------|-------------|
| `.append()` | List | Add element to end of list |
| `.keys()` | Dictionary | Return dictionary keys |
| `type()` | Function | Return data type |
| `len()` | Function | Return length |
| `range()` | Function | Generate number sequence |

## File 3: Lecture 1_Python Basics with Example.ipynb

### Python Built-in Methods
| Method | Type | Description |
|--------|------|-------------|
| `.append()` | List | Add element to list |
| `type()` | Function | Return data type |
| `len()` | Function | Return length |
| `range()` | Function | Generate sequence |

---

# Lec 2: Data Import & EDA

## File 1: lec-2-lab.ipynb

### Pandas Methods
| Method | Type | Description |
|--------|------|-------------|
| `.read_excel()` | Function | Read Excel file into DataFrame |
| `.shape` | Attribute | Return DataFrame dimensions (rows, columns) |
| `.describe()` | Method | Generate summary statistics |
| `.copy()` | Method | Create independent DataFrame copy |
| `.isnull()` | Method | Detect missing values |

## File 2: Lecture 1_Importing Data into Python.ipynb

### Pandas Methods
| Method | Type | Description |
|--------|------|-------------|
| `.read_csv()` | Function | Read CSV file into DataFrame |
| `.read_excel()` | Function | Read Excel file into DataFrame |
| `.info()` | Method | Display DataFrame info |
| `.head()` | Method | Return first 5 rows |
| `.shape` | Attribute | DataFrame dimensions |
| `.columns` | Attribute | Column names |
| `.describe()` | Method | Summary statistics |
| `.isnull()` | Method | Check missing values |

## File 3: Lecture 2_EDA_Descriptive Staistics.ipynb

### Pandas Methods
| Method | Type | Description |
|--------|------|-------------|
| `.read_csv()` | Function | Read CSV file |
| `.info()` | Method | Display DataFrame structure |
| `.head()` | Method | First 5 rows |
| `.tail()` | Method | Last 5 rows |
| `.describe()` | Method | Summary statistics |
| `.dtypes` | Attribute | Column data types |
| `.isnull()` | Method | Check for nulls |
| `.sum()` | Method | Sum of elements |
| `.dropna()` | Method | Remove missing values |
| `.rename()` | Method | Rename columns |
| `.sort_values()` | Method | Sort by column values |
| `.round()` | Method | Round numeric values |
| `.mean()` | Method | Average |
| `.median()` | Method | Median value |
| `.std()` | Method | Standard deviation |
| `.max()` | Method | Maximum value |
| `.skew()` | Method | Measure skewness |
| `.kurt()` | Method | Measure kurtosis |
| `.groupby()` | Method | Group by column |
| `.plot()` | Method | Create plot |

### Matplotlib/Seaborn Functions
| Function | Library | Description |
|----------|---------|-------------|
| `plt.scatter()` | Matplotlib | Create scatter plot |
| `plt.figure()` | Matplotlib | Create figure |
| `plt.title()` | Matplotlib | Set plot title |
| `plt.xlabel()` | Matplotlib | Set x-axis label |
| `plt.ylabel()` | Matplotlib | Set y-axis label |
| `plt.show()` | Matplotlib | Display plot |
| `plt.grid()` | Matplotlib | Add grid |
| `plt.xticks()` | Matplotlib | Set x-axis ticks |
| `plt.yticks()` | Matplotlib | Set y-axis ticks |
| `plt.tight_layout()` | Matplotlib | Adjust layout |
| `sns.histplot()` | Seaborn | Create histogram with KDE |

---

# Lec 3-4: Vectors, Matrices & DataFrames

## File 1: L-3_Vectors_Matrices_DataFrames (2).ipynb

### NumPy Array Methods
| Attribute | Description |
|-----------|-------------|
| `.sum()` | Sum of all elements in array |
| `.mean()` | Average/mean of elements |
| `.max()` | Maximum value |
| `.min()` | Minimum value |
| `.std()` | Standard deviation |
| `.reshape()` | Reshape array to new dimensions |
| `.shape` | Tuple showing array dimensions (rows, columns) |
| `.ndim` | Number of dimensions |
| `.T` | Transpose (flip rows and columns) |

### NumPy Functions
| Function | Description |
|----------|-------------|
| `np.dot()` | Dot product of two vectors/matrices |
| `np.array()` | Create NumPy array from list |
| `np.eye()` | Create identity matrix |
| `np.linalg.det()` | Determinant of matrix |
| `np.linalg.inv()` | Inverse of matrix |

### Pandas Methods
| Attribute | Description |
|-----------|-------------|
| `.iloc[]` | Access rows/columns by integer position |
| `.mean()` | Average of column values |
| `df['column']` | Access column by name |

---

## File 2: lec-3_4.ipynb

### NumPy Methods/Functions
| Attribute | Description |
|-----------|-------------|
| `.sum()` | Sum of elements |
| `.mean()` | Average of elements |
| `.max()` | Maximum element |
| `.min()` | Minimum element |
| `.std()` | Standard deviation |
| `.reshape()` | Reshape array dimensions |
| `.ndim` | Number of dimensions |
| `np.dot()` | Dot product |
| `np.array()` | Create array |

---

## File 3: Lecture-3 and 4_Data Transformation and Numpy Basics.ipynb

### Pandas Methods
| Attribute | Description |
|-----------|-------------|
| `.copy()` | Create independent copy of DataFrame |
| `.drop_duplicates()` | Remove duplicate rows |
| `.pop()` | Remove and return column |
| `.drop()` | Remove rows/columns by index or label |
| `.loc[]` | Access rows/columns by label |
| `.concat()` | Concatenate DataFrames |
| `.get_dummies()` | One-hot encode categorical columns |
| `.cut()` | Bin numeric values into categories |
| `.cat.codes` | Convert categorical to numeric codes |
| `.apply()` | Apply function to each element |
| `df['column']` | Access column by name |
| `.iloc[]` | Access by integer position |

### NumPy Attributes/Methods
| Attribute | Description |
|-----------|-------------|
| `.shape` | Dimensions of array |
| `.ndim` | Number of dimensions |
| `.size` | Total number of elements |
| `.dtype` | Data type of elements |
| `.reshape()` | Change array shape |
| `.flatten()` | Convert to 1D array |

### NumPy Creation Functions
| Function | Description |
|----------|-------------|
| `np.zeros()` | Create array filled with zeros |
| `np.ones()` | Create array filled with ones |
| `np.arange()` | Create array with step intervals |
| `np.linspace()` | Create evenly spaced values |
| `np.random.rand()` | Create random array (0-1) |

### NumPy Math Functions
| Function | Description |
|----------|-------------|
| `np.sqrt()` | Square root |
| `np.exp()` | Exponential |
| `np.sin()` | Sine |
| `np.log()` | Natural logarithm |

### NumPy Aggregation Functions
| Function | Description |
|----------|-------------|
| `np.sum()` | Sum across array or axis |
| `np.mean()` | Mean across array or axis |
| `np.min()` | Minimum value |
| `np.max()` | Maximum value |
| `np.median()` | Median value |
| `np.std()` | Standard deviation |
| `np.var()` | Variance |

### NumPy Stacking Functions
| Function | Description |
|----------|-------------|
| `np.vstack()` | Stack arrays vertically |
| `np.hstack()` | Stack arrays horizontally |

### Matplotlib/Seaborn Methods
| Attribute | Description |
|-----------|-------------|
| `.figure()` | Create new figure/plot |
| `.barplot()` | Create bar chart |
| `.patches` | Access bars/shapes in plot |
| `.get_height()` | Get bar height value |
| `.text()` | Add text annotation to plot |
| `.ylim()` | Set y-axis limits |
| `.show()` | Display plot |
| `.title()` | Set plot title |
| `.ylabel()` | Set y-axis label |
| `.xlabel()` | Set x-axis label |

| Class | Description |
|-------|-------------|
| `LabelEncoder()` | Convert categorical labels to numbers |
| `MinMaxScaler()` | Normalize values to 0-1 range |

---

# Lec 5-6: Simple Linear Regression

## File 1: Lecture 5_6_Simple Linear Regression.ipynb

### Pandas Methods
| Method | Type | Description |
|--------|------|-------------|
| `.read_csv()` | Function | Read CSV file |
| `.shape` | Attribute | DataFrame dimensions |
| `.info()` | Method | Display DataFrame info |
| `.describe()` | Method | Summary statistics |
| `.isnull()` | Method | Check for null values |
| `.sum()` | Method | Sum of elements |
| `.dropna()` | Method | Remove missing values |
| `.select_dtypes()` | Method | Select columns by dtype |
| `.corr()` | Method | Correlation matrix |
| `.round()` | Method | Round values |
| `.map()` | Method | Map values using function |
| `.groupby()` | Method | Group by column |
| `.cut()` | Function | Bin numeric values |
| `.value_counts()` | Method | Count unique values |
| `.concat()` | Function | Concatenate DataFrames |

### Scikit-learn Functions/Classes
| Function/Class | Description |
|----------------|-------------|
| `train_test_split()` | Split data into train/test sets |
| `LinearRegression()` | Linear regression model |
| `mean_squared_error()` | Calculate MSE |
| `r2_score()` | Calculate R² score |
| `mean_absolute_error()` | Calculate MAE |

### Model Methods
| Method | Description |
|--------|-------------|
| `.fit()` | Train model on data |
| `.predict()` | Make predictions |
| `.coef_` | Model coefficients (slope) |
| `.intercept_` | Model intercept |

### Matplotlib/Seaborn Functions
| Function | Library | Description |
|----------|---------|-------------|
| `plt.figure()` | Matplotlib | Create figure |
| `plt.scatter()` | Matplotlib | Create scatter plot |
| `plt.plot()` | Matplotlib | Plot line |
| `plt.title()` | Matplotlib | Set title |
| `plt.xlabel()` | Matplotlib | Set x label |
| `plt.ylabel()` | Matplotlib | Set y label |
| `plt.legend()` | Matplotlib | Add legend |
| `plt.grid()` | Matplotlib | Add grid |
| `plt.show()` | Matplotlib | Display plot |
| `plt.axhline()` | Matplotlib | Add horizontal line |
| `plt.ylim()` | Matplotlib | Set y-axis limits |
| `sns.heatmap()` | Seaborn | Create heatmap |
| `sns.pairplot()` | Seaborn | Plot pairwise relationships |
| `sns.scatterplot()` | Seaborn | Create scatter plot |
| `sns.histplot()` | Seaborn | Create histogram |
| `sns.kdeplot()` | Seaborn | Create KDE plot |

### StatsModels Functions
| Function | Description |
|----------|-------------|
| `sm.qqplot()` | Create Q-Q plot |
| `sm.add_constant()` | Add constant column for VIF |
| `variance_inflation_factor()` | Calculate VIF |

### Scipy Functions
| Function | Description |
|----------|-------------|
| `scipy.stats.pearsonr()` | Pearson correlation & p-value |

## File 2: Lecture 5_Simple Linear Regression Example.ipynb

### Core Functions/Methods (same as File 1)
- `train_test_split()`, `LinearRegression()`, `.fit()`, `.predict()`
- `mean_squared_error()`, `r2_score()`
- `sns.heatmap()`, `sns.scatterplot()`, `sns.histplot()`, `sns.kdeplot()`

---

# Lec 7: Multiple Linear Regression

## File 1: Lecture 7_Multiple Linear Regression.ipynb

### Pandas Methods
| Method | Type | Description |
|--------|------|-------------|
| `.read_csv()` | Function | Read CSV file |
| `.shape` | Attribute | DataFrame dimensions |
| `.info()` | Method | Display info |
| `.describe()` | Method | Summary statistics |
| `.isnull()` | Method | Check null values |
| `.sum()` | Method | Sum of elements |
| `.dropna()` | Method | Remove nulls |
| `.select_dtypes()` | Method | Select by dtype |
| `.corr()` | Method | Correlation matrix |
| `.round()` | Method | Round values |
| `.map()` | Method | Map values |
| `.groupby()` | Method | Group by column |
| `.cut()` | Function | Bin values |

### Scikit-learn Functions/Classes
| Function/Class | Description |
|----------------|-------------|
| `train_test_split()` | Split train/test data |
| `LinearRegression()` | Linear regression model |
| `mean_squared_error()` | Calculate MSE |
| `r2_score()` | Calculate R² score |
| `mean_absolute_error()` | Calculate MAE |

### Model Methods
| Method | Description |
|--------|-------------|
| `.fit()` | Train model |
| `.predict()` | Make predictions |
| `.coef_` | Coefficients |
| `.intercept_` | Intercept |

### Matplotlib/Seaborn Functions
| Function | Library | Description |
|----------|---------|-------------|
| `sns.heatmap()` | Seaborn | Create heatmap |
| `sns.pairplot()` | Seaborn | Pairwise relationships |

### StatsModels Functions
| Function | Description |
|----------|-------------|
| `sm.add_constant()` | Add constant for regression |
| `variance_inflation_factor()` | Calculate VIF |

---

## Summary Table: Methods by Category

### Data Loading & Inspection
| Method | Used in Lectures |
|--------|-----------------|
| `read_csv()` | Lec 2, 5-6, 7 |
| `read_excel()` | Lec 2 |
| `.shape` | Lec 2, 5-6, 7 |
| `.info()` | Lec 2, 5-6, 7 |
| `.head()` | Lec 2 |
| `.tail()` | Lec 2 |
| `.describe()` | Lec 2, 5-6, 7 |

### Data Cleaning
| Method | Used in Lectures |
|--------|-----------------|
| `.isnull()` | Lec 2, 5-6, 7 |
| `.dropna()` | Lec 2, 5-6, 7 |
| `.copy()` | Lec 2 |
| `.rename()` | Lec 2 |

### Statistical Analysis
| Method | Used in Lectures |
|--------|-----------------|
| `.mean()`, `.median()`, `.std()`, `.max()`, `.min()` | Lec 2 |
| `.skew()`, `.kurt()` | Lec 2 |
| `.corr()` | Lec 3-4, 5-6, 7 |
| `.groupby()` | Lec 2, 5-6, 7 |

### Machine Learning
| Method | Used in Lectures |
|--------|-----------------|
| `train_test_split()` | Lec 5-6, 7 |
| `LinearRegression()` | Lec 5-6, 7 |
| `mean_squared_error()`, `r2_score()`, `mean_absolute_error()` | Lec 5-6, 7 |
| `variance_inflation_factor()` | Lec 5-6, 7 |

### Visualization
| Method | Used in Lectures |
|--------|-----------------|
| `sns.heatmap()` | Lec 3-4, 5-6, 7 |
| `sns.pairplot()` |  Lec 3-4, 5-6, 7 |
| `sns.scatterplot()` | Lec 2, 5-6 |
| `sns.histplot()` | Lec 2, 5-6 |
| `sns.kdeplot()` | Lec 5-6 |
| `plt.scatter()`, `plt.plot()` | Lec 2, 5-6 |
| `plt.figure()`, `plt.show()` | Lec 2, 5-6 |
