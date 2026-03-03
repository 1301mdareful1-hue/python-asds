# Unique Methods & Short Examples

## Python Built-ins
| Method/Function | Short example |
|---|---|
| `type()` | `type(3.14)` |
| `len()` | `len(['a', 'b', 'c'])` |
| `range()` | `list(range(1, 5))` |
| `sum()` | `sum([10, 20, 30])` |

## List & Dictionary
| Method/Function | Short example |
|---|---|
| `.append()` | `names.append('Eve')` |
| `.remove()` | `names.remove('Bob')` |
| `.pop()` | `names.pop(0)` |
| `.keys()` | `student.keys()` |

## Pandas
| Method/Function | Short example |
|---|---|
| `pd.read_csv()` | `df = pd.read_csv('data.csv')` |
| `pd.read_excel()` | `df = pd.read_excel('data.xlsx')` |
| `.shape` | `df.shape` |
| `.columns` | `df.columns` |
| `.dtypes` | `df.dtypes` |
| `.info()` | `df.info()` |
| `.head()` | `df.head(3)` |
| `.tail()` | `df.tail(3)` |
| `.describe()` | `df.describe()` |
| `.copy()` | `df2 = df.copy()` |
| `.isnull()` | `df.isnull().sum()` |
| `.dropna()` | `df = df.dropna()` |
| `.rename()` | `df = df.rename(columns={'A':'Age'})` |
| `.sort_values()` | `df.sort_values(by='Salary')` |
| `.round()` | `df.round(2)` |
| `.mean()` | `df['Salary'].mean()` |
| `.median()` | `df['Salary'].median()` |
| `.std()` | `df['Salary'].std()` |
| `.max()` | `df['Age'].max()` |
| `.min()` | `df['Age'].min()` |
| `.skew()` | `df['Age'].skew()` |
| `.kurt()` | `df['Age'].kurt()` |
| `.groupby()` | `df.groupby('Gender')['Salary'].mean()` |
| `.plot()` | `df['Salary'].plot(kind='hist')` |
| `.drop_duplicates()` | `df.drop_duplicates(subset=['Name'])` |
| `.drop()` | `df.drop(columns=['City'])` |
| `.loc[]` | `df.loc[0, 'Salary']` |
| `.iloc[]` | `df.iloc[0, 1]` |
| `pd.concat()` | `pd.concat([df1, df2], axis=0)` |
| `pd.get_dummies()` | `pd.get_dummies(df, columns=['City'])` |
| `pd.cut()` | `pd.cut(df['Age'], bins=[20,30,40])` |
| `.cat.codes` | `df['code'] = df['grade'].cat.codes` |
| `.apply()` | `df['Pass'] = df['Score'].apply(lambda x: x >= 60)` |
| `.map()` | `df['Gender_Code'] = df['Gender'].map({'Male':1,'Female':0})` |
| `.select_dtypes()` | `df.select_dtypes(include=['number'])` |
| `.corr()` | `df.corr(numeric_only=True)` |
| `.value_counts()` | `df['Gender'].value_counts()` |

## NumPy
| Method/Function | Short example |
|---|---|
| `np.array()` | `arr = np.array([1, 2, 3])` |
| `np.dot()` | `np.dot([1,2], [3,4])` |
| `np.eye()` | `np.eye(3)` |
| `np.linalg.det()` | `np.linalg.det(np.array([[1,2],[3,4]]))` |
| `np.linalg.inv()` | `np.linalg.inv(np.array([[1,2],[3,4]]))` |
| `.reshape()` | `arr.reshape(3, 1)` |
| `.ndim` | `arr.ndim` |
| `.size` | `arr.size` |
| `.dtype` | `arr.dtype` |
| `.T` | `mat.T` |
| `.flatten()` | `mat.flatten()` |
| `np.zeros()` | `np.zeros((2,3))` |
| `np.ones()` | `np.ones((2,2))` |
| `np.arange()` | `np.arange(0, 10, 2)` |
| `np.linspace()` | `np.linspace(0, 1, 5)` |
| `np.random.rand()` | `np.random.rand(2, 2)` |
| `np.sqrt()` | `np.sqrt(np.array([1,4,9]))` |
| `np.exp()` | `np.exp(np.array([1,2]))` |
| `np.sin()` | `np.sin(np.array([0, np.pi/2]))` |
| `np.log()` | `np.log(np.array([1, np.e]))` |
| `np.sum()` | `np.sum(arr)` |
| `np.mean()` | `np.mean(arr)` |
| `np.min()` | `np.min(arr)` |
| `np.max()` | `np.max(arr)` |
| `np.median()` | `np.median(arr)` |
| `np.std()` | `np.std(arr)` |
| `np.var()` | `np.var(arr)` |
| `np.vstack()` | `np.vstack((a, b))` |
| `np.hstack()` | `np.hstack((a, b))` |

## Scikit-learn / Stats / Modeling
| Method/Function | Short example |
|---|---|
| `train_test_split()` | `X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2)` |
| `LinearRegression()` | `model = LinearRegression()` |
| `.fit()` | `model.fit(X_train, y_train)` |
| `.predict()` | `y_pred = model.predict(X_test)` |
| `.coef_` | `model.coef_` |
| `.intercept_` | `model.intercept_` |
| `mean_squared_error()` | `mean_squared_error(y_test, y_pred)` |
| `r2_score()` | `r2_score(y_test, y_pred)` |
| `mean_absolute_error()` | `mean_absolute_error(y_test, y_pred)` |
| `LabelEncoder()` | `codes = LabelEncoder().fit_transform(df['City'])` |
| `MinMaxScaler()` | `scaled = MinMaxScaler().fit_transform(df[['A','B']])` |
| `scipy.stats.pearsonr()` | `r, p = scipy.stats.pearsonr(df['X'], df['Y'])` |
| `sm.add_constant()` | `X2 = sm.add_constant(X)` |
| `sm.qqplot()` | `sm.qqplot(residuals, line='45')` |
| `variance_inflation_factor()` | `variance_inflation_factor(X2.values, 1)` |

## Matplotlib / Seaborn
| Method/Function | Short example |
|---|---|
| `plt.figure()` | `plt.figure(figsize=(6,4))` |
| `plt.scatter()` | `plt.scatter(df['x'], df['y'])` |
| `plt.plot()` | `plt.plot(x, y_pred)` |
| `plt.title()` | `plt.title('My Plot')` |
| `plt.xlabel()` | `plt.xlabel('X')` |
| `plt.ylabel()` | `plt.ylabel('Y')` |
| `plt.legend()` | `plt.legend()` |
| `plt.grid()` | `plt.grid(True)` |
| `plt.show()` | `plt.show()` |
| `plt.axhline()` | `plt.axhline(y=0, color='red')` |
| `plt.ylim()` | `plt.ylim(0, 100)` |
| `plt.xticks()` | `plt.xticks(rotation=45)` |
| `plt.yticks()` | `plt.yticks(rotation=45)` |
| `plt.tight_layout()` | `plt.tight_layout()` |
| `sns.heatmap()` | `sns.heatmap(df.corr(numeric_only=True), annot=True)` |
| `sns.pairplot()` | `sns.pairplot(df)` |
| `sns.scatterplot()` | `sns.scatterplot(data=df, x='x', y='y')` |
| `sns.histplot()` | `sns.histplot(df['Age'], kde=True)` |
| `sns.kdeplot()` | `sns.kdeplot(df['Salary'])` |
| `sns.barplot()` | `sns.barplot(data=df, x='Grade', y='Score')` |
