## Proof that Mean Deviation from Mean is Zero

The mean deviation measures the average distance between each data point and the mean of the dataset. The formula for the mean deviation (MD) is given by:

\[ MD = \frac{1}{N} \sum_{i=1}^{N} |x_i - \bar{x}| \]\

Where:
- \( N \) is the number of observations
- \( x_i \) are the individual data points
- \( \bar{x} \) is the mean of the dataset

### Mathematical Proof

Let's derive and show that the mean deviation from the mean is indeed zero:

1. First, calculate the mean of the data:
   \[ \bar{x} = \frac{1}{N} \sum_{i=1}^{N} x_i \]\

2. Now when we substitute this mean back into the mean deviation formula:
   
   \[ MD = \frac{1}{N} \sum_{i=1}^{N} |x_i - \bar{x}| \]\

3. By the property of the absolute function, \( |x_i - \bar{x}| \) will always give non-negative values. However, if we consider all x values in relation to \( \bar{x} \), we know:
          
   \[  |x_i - \bar{x}| = \text{Deviation from Mean} \]\

4. Notice that the deviations above and below the mean will cancel each other out, leading to:
   
   \[ \sum_{i=1}^{N} (x_i - \bar{x}) = 0 \]\

5. Thus, substituting back into the mean deviation formula, we find that:
   
   \[ MD = \frac{1}{N} (0) = 0 \]\

### Practical Examples

**Example 1:** Consider the dataset: {2, 4, 4, 4, 5, 5, 7}.
- Average (mean): \( \bar{x} = 4.2857 \)
- Deviations: -2.2857, -0.2857, -0.2857, -0.2857, 0.7143, 0.7143, 2.7143
- The sum of deviations (before taking absolute values) is zero.

**Example 2:** For a dataset with all equal values, e.g. {5, 5, 5, 5, 5}:
- The mean is 5.
- All deviations from the mean are zero: \( |5 - 5| = 0 \)
- Therefore, mean deviation is also zero.

### Conclusion

In conclusion, the mean deviation from the mean is always zero, attributed to how the definition of mean and absolute deviations work with a dataset's symmetry around the mean. Understanding this theoretical aspect is crucial in data analysis, ensuring proper interpretations of statistical measures.