# Statistics Toolbox
For any given statistical method/function/tool, there are a few important questions to ask. (I LIE backwards)
1. What is the formal definition? (**E**quation)
2. When should it be used? (**I**nput Data)
3. When does it break? (**L**imitations)
4. What do the results mean? (**I**nterpretation)

## Summary Statistics
### Mean 
**Definition**: Sum of all values divided by the number of elements in a given set. 
$$\bar{x}=\frac{\sum_{i=1}^{n}x_i}{n}$$

````{tab-set}
```{tab-item} Input Data
Numerical (although more interpretable on continuous data)  
```
```{tab-item} Limitations
Sensitive to outliers &rarr; the **mean** can be skewed greatly by a small number of outliers.  
```
```{tab-item} Interpretation
The most common or 'typical' value in a distribution of values.
```
````

```{note}
There are many variations to the mean for different use cases. For instance, the weighted mean uses a user-assigned 'weight' to each value. Another is the trimmed mean, where the smallest and largest $p$ values are removed prior to calculating the mean.
```

#### Weighted Mean
**Definition**: Variation of the mean where user-specified weights are applied to individual values.  
$$\bar{x}_w=\frac{\sum_{i=1}^{n}w_ix_i}{\sum_{i=1}^{n}w_i}$$
**Input Data**: Numerical  
**Limitations**: Requires definition of weights which may introduce bias. 
**Interpretation**: The estimate of the most 'typical' value.

#### Trimmed Mean 
**Definition**: Variation of the mean where the smallest and largest $p$ values are removed. 
$$\bar{x}=\frac{\sum_{i=p+1}^{n-p}x_{(i)}}{n-2p}$$
**Input Data**: Numerical   
**Limitations**: Potentially cuts outliers out of the distribution, but may also introduce bias.   
**Interpretation**: Estimate of the most typical value in a distribution.  

### Median 
**Definition**: The *middle* value in a sorted list of values. 
$$Med(X)=\begin{cases}
X[\frac{n+1}{2}], & \text{if } n \text{ is odd}\\

\frac{X[\frac{n}{2}]+X[\frac{n}{2}+1]}{2}, & \text{if } n \text{ is even}
\end{cases}$$   
**Input Data**: Numerical  
**Limitations**:   
**Interpretation**: A robust estimate of location since it isn't influenced by outliers as strongly as mean.   

```{note}
Like weighted means, there are also weighted medians.
```

### Variance and Standard Deviation 
**Definition**:   
**Input Data**:   
**Limitations**:   
**Interpretation**:  