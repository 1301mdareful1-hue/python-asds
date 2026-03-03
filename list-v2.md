# Methods with Description and Example

## Python Built-ins
| Method/Function | Short description | Short example |
|---|---|---|
| `type()` | Returns the data type of a value | `type(3.14)` |
| `len()` | Returns number of items | `len(['a', 'b', 'c'])` |
| `range()` | Generates a sequence of integers | `list(range(1, 5))` |
| `sum()` | Adds numeric items together | `sum([10, 20, 30])` |

## List & Dictionary
| Method/Function | Short description | Short example |
|---|---|---|
| `.append()` | Adds an item at list end | `names.append('Eve')` |
| `.remove()` | Removes first matching item | `names.remove('Bob')` |
| `.pop()` | Removes item by index and returns it | `names.pop(0)` |
| `.keys()` | Returns all dictionary keys | `student.keys()` |

## Pandas
| Method/Function | Short description | Short example |
|---|---|---|
| `pd.read_csv()` | Loads CSV into DataFrame | `df = pd.read_csv('data.csv')` |
| `pd.read_excel()` | Loads Excel into DataFrame | `df = pd.read_excel('data.xlsx')` |
| `.shape` | Gives rows and columns count | `df.shape` |
| `.columns` | Shows column names | `df.columns` |
| `.dtypes` | Shows data types per column | `df.dtypes` |
| `.info()` | Prints structure and null counts | `df.info()` |
| `.head()` | Shows first rows | `df.head(3)` |
| `.tail()` | Shows last rows | `df.tail(3)` |
| `.describe()` | Summary stats for numeric columns | `df.describe()` |
| `.copy()` | Creates independent DataFrame copy | `df2 = df.copy()` |
| `.isnull()` | Marks missing values as True/False | `df.isnull().sum()` |
| `.dropna()` | Removes rows/columns with nulls | `df = df.dropna()` |
| `.rename()` | Renames columns or index labels | `df = df.rename(columns={'A':'Age'})` |
| `.sort_values()` | Sorts rows by column values | `df.sort_values(by='Salary')` |
| `.round()` | Rounds numeric values | `df.round(2)` |
| `.mean()` | Computes average | `df['Salary'].mean()` |
| `.median()` | Computes middle value | `df['Salary'].median()` |
| `.std()` | Computes standard deviation | `df['Salary'].std()` |
| `.max()` | Returns largest value | `df['Age'].max()` |
| `.min()` | Returns smallest value | `df['Age'].min()` |
| `.skew()` | Measures distribution asymmetry | `df['Age'].skew()` |
| `.kurt()` | Measures tailedness/peakedness | `df['Age'].kurt()` |
| `.groupby()` | Groups rows for aggregated analysis | `df.groupby('Gender')['Salary'].mean()` |
| `.plot()` | Quick plotting from DataFrame/Series | `df['Salary'].plot(kind='hist')` |
| `.drop_duplicates()` | Removes duplicate rows | `df.drop_duplicates(subset=['Name'])` |
| `.drop()` | Removes selected rows/columns | `df.drop(columns=['City'])` |
| `.loc[]` | Label-based row/column selection | `df.loc[0, 'Salary']` |
| `.iloc[]` | Position-based row/column selection | `df.iloc[0, 1]` |
| `pd.concat()` | Combines DataFrames vertically/horizontally | `pd.concat([df1, df2], axis=0)` |
| `pd.get_dummies()` | One-hot encodes categorical columns | `pd.get_dummies(df, columns=['City'])` |
| `pd.cut()` | Bins continuous values into categories | `pd.cut(df['Age'], bins=[20,30,40])` |
| `.cat.codes` | Converts category labels to integer codes | `df['code'] = df['grade'].cat.codes` |
| `.apply()` | Applies function across values | `df['Pass'] = df['Score'].apply(lambda x: x >= 60)` |
| `.map()` | Maps values via dictionary/function | `df['Gender_Code'] = df['Gender'].map({'Male':1,'Female':0})` |
| `.select_dtypes()` | Selects columns by datatype | `df.select_dtypes(include=['number'])` |
| `.corr()` | Correlation matrix of numeric columns | `df.corr(numeric_only=True)` |
| `.value_counts()` | Counts unique values frequency | `df['Gender'].value_counts()` |

## NumPy
| Method/Function | Short description | Short example |
|---|---|---|
| `np.array()` | Creates NumPy array | `arr = np.array([1, 2, 3])` |
| `np.dot()` | Computes dot product | `np.dot([1,2], [3,4])` |
| `np.eye()` | Creates identity matrix | `np.eye(3)` |
| `np.linalg.det()` | Computes matrix determinant | `np.linalg.det(np.array([[1,2],[3,4]]))` |
| `np.linalg.inv()` | Computes matrix inverse | `np.linalg.inv(np.array([[1,2],[3,4]]))` |
| `.reshape()` | Changes array dimensions | `arr.reshape(3, 1)` |
| `.ndim` | Number of dimensions | `arr.ndim` |
| `.size` | Number of total elements | `arr.size` |
| `.dtype` | Data type of elements | `arr.dtype` |
| `.T` | Matrix transpose | `mat.T` |
| `.flatten()` | Converts to 1D array | `mat.flatten()` |
| `np.zeros()` | Array filled with zeros | `np.zeros((2,3))` |
| `np.ones()` | Array filled with ones | `np.ones((2,2))` |
| `np.arange()` | Range of evenly spaced integers | `np.arange(0, 10, 2)` |
| `np.linspace()` | Fixed count of evenly spaced values | `np.linspace(0, 1, 5)` |
| `np.random.rand()` | Random numbers in [0,1) | `np.random.rand(2, 2)` |
| `np.sqrt()` | Square root element-wise | `np.sqrt(np.array([1,4,9]))` |
| `np.exp()` | Exponential element-wise | `np.exp(np.array([1,2]))` |
| `np.sin()` | Sine element-wise | `np.sin(np.array([0, np.pi/2]))` |
| `np.log()` | Natural log element-wise | `np.log(np.array([1, np.e]))` |
| `np.sum()` | Sum of values | `np.sum(arr)` |
| `np.mean()` | Mean of values | `np.mean(arr)` |
| `np.min()` | Minimum value | `np.min(arr)` |
| `np.max()` | Maximum value | `np.max(arr)` |
| `np.median()` | Median value | `np.median(arr)` |
| `np.std()` | Standard deviation | `np.std(arr)` |
| `np.var()` | Variance | `np.var(arr)` |
| `np.vstack()` | Vertical stacking of arrays | `np.vstack((a, b))` |
| `np.hstack()` | Horizontal stacking of arrays | `np.hstack((a, b))` |

## Scikit-learn / Stats / Modeling
| Method/Function | Short description | Short example |
|---|---|---|
| `train_test_split()` | Splits data into train/test sets | `X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2)` |
| `LinearRegression()` | Creates linear regression model | `model = LinearRegression()` |
| `.fit()` | Trains model with data | `model.fit(X_train, y_train)` |
| `.predict()` | Generates predictions | `y_pred = model.predict(X_test)` |
| `.coef_` | Model slope coefficients | `model.coef_` |
| `.intercept_` | Model intercept value | `model.intercept_` |
| `mean_squared_error()` | Average squared prediction error | `mean_squared_error(y_test, y_pred)` |
| `r2_score()` | Proportion of explained variance | `r2_score(y_test, y_pred)` |
| `mean_absolute_error()` | Average absolute prediction error | `mean_absolute_error(y_test, y_pred)` |
| `LabelEncoder()` | Encodes labels as integers | `codes = LabelEncoder().fit_transform(df['City'])` |
| `MinMaxScaler()` | Scales values to [0,1] range | `scaled = MinMaxScaler().fit_transform(df[['A','B']])` |
| `scipy.stats.pearsonr()` | Pearson correlation and p-value | `r, p = scipy.stats.pearsonr(df['X'], df['Y'])` |
| `sm.add_constant()` | Adds intercept column for stats model | `X2 = sm.add_constant(X)` |
| `sm.qqplot()` | Q-Q plot for normality check | `sm.qqplot(residuals, line='45')` |
| `variance_inflation_factor()` | Measures multicollinearity | `variance_inflation_factor(X2.values, 1)` |

## Matplotlib / Seaborn
| Method/Function | Short description | Short example |
|---|---|---|
| `plt.figure()` | Starts a new figure | `plt.figure(figsize=(6,4))` |
| `plt.scatter()` | Scatter plot | `plt.scatter(df['x'], df['y'])` |
| `plt.plot()` | Line plot | `plt.plot(x, y_pred)` |
| `plt.title()` | Sets plot title | `plt.title('My Plot')` |
| `plt.xlabel()` | Sets x-axis label | `plt.xlabel('X')` |
| `plt.ylabel()` | Sets y-axis label | `plt.ylabel('Y')` |
| `plt.legend()` | Displays legend | `plt.legend()` |
| `plt.grid()` | Adds grid lines | `plt.grid(True)` |
| `plt.show()` | Renders the plot | `plt.show()` |
| `plt.axhline()` | Adds horizontal reference line | `plt.axhline(y=0, color='red')` |
| `plt.ylim()` | Sets y-axis limits | `plt.ylim(0, 100)` |
| `plt.xticks()` | Controls x ticks/rotation | `plt.xticks(rotation=45)` |
| `plt.yticks()` | Controls y ticks/rotation | `plt.yticks(rotation=45)` |
| `plt.tight_layout()` | Adjusts spacing to prevent overlap | `plt.tight_layout()` |
| `sns.heatmap()` | Heatmap for matrix/correlation | `sns.heatmap(df.corr(numeric_only=True), annot=True)` |
| `sns.pairplot()` | Pairwise variable relationship plots | `sns.pairplot(df)` |
| `sns.scatterplot()` | Styled scatter plot | `sns.scatterplot(data=df, x='x', y='y')` |
| `sns.histplot()` | Histogram (optional KDE) | `sns.histplot(df['Age'], kde=True)` |
| `sns.kdeplot()` | Kernel density estimate plot | `sns.kdeplot(df['Salary'])` |
| `sns.barplot()` | Categorical bar plot with estimator | `sns.barplot(data=df, x='Grade', y='Score')` |
