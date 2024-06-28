### Univariate Analysis

- Categorical Analysis
    - Count Plot: value counts
    - Pie Chart: percentage counts
- Numerical Analysis
    - Histogram: range of values and their frequency (distribution)
    - Dist Plot: Kind of histogram with KDE (Kernel Density Estimation)
    - Box Plot: 5 number summary (min, 25%, 50%, 75%, max)
    - Violin Plot: Box plot with KDE
    - Pair Plot: Pairwise relationship between numerical columns
    - Heat Map: Correlation between numerical columns


### Bivariate Analysis
- Scatter Plot: Relationship between two numerical columns
- Bar Plot: Relationship between one numerical and one categorical column
- Box Plot: Relationship between one numerical and one categorical column
- Dist Plot: Relationship between one numerical and one categorical column
- Heat Map: Correlation between numerical columns
- Pair Plot: Collection of scatter plots between numerical columns
- Line Plot: Relationship between two numerical columns, with one being time

### Feature Engineering
- Feature Transformation
    - Normalization
    - Standardization
    - Log Transformation
    - Polynomial Transformation
    - Binning
- Feature Creation
    - Interaction Features
    - Polynomial Features
    - Domain Specific Features
- Feature Selection
    - Filter Methods
    - Wrapper Methods
    - Embedded Methods
- Feature Scaling
    - Min-Max Scaler
    - Standard Scaler
    - Robust Scaler
    - Normalizer

### Feature Scaling
- Standardization (z-score normalization)
    - Geometric Intution: Mean centering and scaling by standard deviation
    - Formula: x' = (x - mean(x)) / std(x)
    - Conclusion: mean = 0, std = 1
    - Outlier won't be removed but will be scaled
    - When to use it
        - KMeans
        - KNN
        - PCA
        - ANN
        - Gradient Descent

- Normalization
    - Eliminate the units without changing the range of values or losing information
    - Formula: x' = (x - min(x)) / (max(x) - min(x))
    - Conclusion: range = [0, 1]
    - To handle outliers we can use RobustScaler

- Standardization vs Normalization
    - Is feature scaling required
        - Yes, when the algorithm is distance based
        - No, when the algorithm is tree based
    - If you know the range of your numerical quantity then use Min-Max Scaler
    - No idea about the range then use Standard Scaler
    
