| Topic | Function | Short Description | Example |
|---|---|---|---|
| Data loading | pd.read_csv() | Load CSV file into DataFrame | df = pd.read_csv("data.csv") |
| Data loading | pd.read_excel() | Load Excel file into DataFrame | df = pd.read_excel("students.xlsx") |
| Quick view | df.head() | Show first 5 rows | df.head() |
| Data info | df.info() | Column names, types, non-null count | df.info() |
| Data summary | df.describe() | Summary stats for numeric columns | df.describe() |
| Mean | df["Salary"].mean() | Average value | df["Salary"].mean() |
| Median | df["Salary"].median() | Middle value | df["Salary"].median() |
| Max | df["Salary"].max() | Largest value | df["Salary"].max() |
| Missing data check | df.isnull() | True/False missing-value map | df.isnull() |
| Missing data count | df.isnull().sum() | Missing count per column | df.isnull().sum() |
| Data cleaning (remove NA) | df.dropna() | Remove rows with missing values | df_clean = df.dropna() |
| Data cleaning (fill NA) | df.fillna() | Fill missing values | df["Age"] = df["Age"].fillna(df["Age"].mean()) |
| Rename columns | df.rename() | Rename one or more columns | df = df.rename(columns={"old_name":"new_name"}) |
| Drop column | df.drop(axis=1) | Remove a column | df = df.drop("UnwantedCol", axis=1) |
| Drop duplicate rows | df.drop_duplicates() | Remove duplicate records | df = df.drop_duplicates() |
| Data formatting | df["col"].astype() | Convert datatype | df["Age"] = df["Age"].astype("int") |
| Data formatting | pd.to_datetime() | Convert to datetime | df["Date"] = pd.to_datetime(df["Date"]) |
| Correlation | df.corr() | Pairwise numeric correlations | df.corr() |
| Variance | df["Salary"].var() | Spread around mean | df["Salary"].var() |
| Standard deviation | df["Salary"].std() | Dispersion (sqrt of variance) | df["Salary"].std() |
| Coefficient of variation | std/mean | Relative spread as percentage | (df["Salary"].std()/df["Salary"].mean())*100 |
| Sort data | df.sort_values() | Sort by column value | df.sort_values("Salary", ascending=False) |
| Group summary | df.groupby() | Aggregate by category | df.groupby("Dept")["Salary"].mean() |

## Chart and graph functions

| Chart Type | Function | Short Description | Example |
|---|---|---|---|
| Histogram | plt.hist() or sns.histplot() | Distribution of one variable | sns.histplot(df["Salary"], kde=True) |
| Bar chart | sns.barplot() | Compare category averages | sns.barplot(data=df, x="Dept", y="Salary") |
| Heatmap | sns.heatmap() | Matrix color map (often correlation) | sns.heatmap(df.corr(), annot=True, cmap="coolwarm") |
| Line chart | plt.plot() | Trend over index/time | plt.plot(df["Date"], df["Sales"]) |
| Scatter plot | plt.scatter() or sns.scatterplot() | Relation between two numeric vars | sns.scatterplot(data=df, x="Experience", y="Salary") |
| Box plot | sns.boxplot() | Outliers and spread | sns.boxplot(data=df, y="Salary") |

## Linear regression essentials

| Topic | Function | Short Description | Example |
|---|---|---|---|
| Split data | train_test_split() | Train/test split | X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42) |
| Model creation | LinearRegression() | Linear regression model | model = LinearRegression() |
| Model training | model.fit() | Fit model on training data | model.fit(X_train, y_train) |
| Prediction | model.predict() | Predict target values | y_pred = model.predict(X_test) |
| Coefficients | model.coef_ | Feature effect on target | model.coef_ |
| Intercept | model.intercept_ | Constant term | model.intercept_ |
| R squared | r2_score() | Goodness of fit | r2_score(y_test, y_pred) |
| MAE | mean_absolute_error() | Average absolute error | mean_absolute_error(y_test, y_pred) |
| MSE | mean_squared_error() | Average squared error | mean_squared_error(y_test, y_pred) |
| RMSE | sqrt(MSE) | Error in target unit | np.sqrt(mean_squared_error(y_test, y_pred)) |
