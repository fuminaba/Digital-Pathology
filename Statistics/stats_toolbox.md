# Statistics Toolbox
For any given statistical method/function/tool, there are a few important questions to ask. (IDLE)
1. **I**nterpretation - what do the results mean?
2. **D**ata Type - what is the input data?
3. **L**imitations - when does this method break?
4. **E**quation - what is the formal definition?

## Summary Statistics
### Measures of Center


#### Mean 
**Definition**: Sum of all values divided by the number of elements in a given set.  
\begin{equation}
    \bar{x}=\frac{\sum_{i=1}^{n}x_i}{n}
\end{equation}

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
There are many variations to the mean for different use cases. 
For instance, the weighted mean uses a user-assigned 'weight' to each value. 
Another is the trimmed mean, where the smallest and largest 'p' values are removed prior to calculating the mean.
```

#### Weighted Mean
**Definition**: Variation of the mean where user-specified weights are applied to individual values.  
\begin{equation}
    \bar{x}_w=\frac{\sum_{i=1}^{n}w_ix_i}{\sum_{i=1}^{n}w_i}
\end{equation}
**Input Data**: Numerical  
**Limitations**: Requires definition of weights which may introduce bias. 
**Interpretation**: The estimate of the most 'typical' value.
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
#### Trimmed Mean 
**Definition**: Variation of the mean where the smallest and largest $p$ values are removed. 
\begin{equation}
    \bar{x}=\frac{\sum_{i=p+1}^{n-p}x_{(i)}}{n-2p}
\end{equation}
**Input Data**: Numerical   
**Limitations**: Potentially cuts outliers out of the distribution, but may also introduce bias.   
**Interpretation**: Estimate of the most typical value in a distribution.  

#### Median 
**Definition**: The *middle* value in a sorted list of values.
\begin{equation} 
    Med(X)=
    \begin{cases}
        X[\frac{n+1}{2}], & \text{if } n \text{ is odd}\\

        \frac{X[\frac{n}{2}]+X[\frac{n}{2}+1]}{2}, & \text{if } n \text{ is even}
    \end{cases}   
\end{equation}
**Input Data**: Numerical  
**Limitations**:   
**Interpretation**: A robust estimate of location since it isn't influenced by outliers as strongly as mean.   

```{note}
Like weighted means, there are also weighted medians.
```

### Measures of Spread
#### Variance 

#### Standard Deviation 
**Definition**:   
**Input Data**:   
**Limitations**:   
**Interpretation**:  