# Course - Unsupervised Learning 

##### NOTE: 
1. Your code MUST execute without any errors. 
2. You can add more lines in your code as required.

## Section 1: Clustering: K-mean Clustering

### Question 1 
**The dataset is loaded for you. Perform the following tasks:**  
1. The dataset contains milk composition from different mammals. You are required to cluster the observations using K mean clustering.  
2. Plot out the distributions (histogram) of each of the variables (columns) and see how they behave.  
3. Use k=3, 5, 10, 15, 20. Plot the sum of squares values as a chart and select the appropriate value of K. 


```R
library(cluster.datasets)
data(all.mammals.milk.1956)
head(all.mammals.milk.1956)
```


<table>
<thead><tr><th scope=col>name</th><th scope=col>water</th><th scope=col>protein</th><th scope=col>fat</th><th scope=col>lactose</th><th scope=col>ash</th></tr></thead>
<tbody>
	<tr><td>Horse    </td><td>90.1     </td><td>2.6      </td><td>1.0      </td><td>6.9      </td><td>0.35     </td></tr>
	<tr><td>Orangutan</td><td>88.5     </td><td>1.4      </td><td>3.5      </td><td>6.0      </td><td>0.24     </td></tr>
	<tr><td>Monkey   </td><td>88.4     </td><td>2.2      </td><td>2.7      </td><td>6.4      </td><td>0.18     </td></tr>
	<tr><td>Donkey   </td><td>90.3     </td><td>1.7      </td><td>1.4      </td><td>6.2      </td><td>0.40     </td></tr>
	<tr><td>Hippo    </td><td>90.4     </td><td>0.6      </td><td>4.5      </td><td>4.4      </td><td>0.10     </td></tr>
	<tr><td>Camel    </td><td>87.7     </td><td>3.5      </td><td>3.4      </td><td>4.8      </td><td>0.71     </td></tr>
</tbody>
</table>




```R

```


```R

```


```R

```

### Good Job! You are done with the section!

## Section 2: Clustering: Hierarchal Clustering

### Question 1 
**The dataset is loaded for you. Perform the following tasks:**  
You have data for price. indices from EU stock market. You wish to pair trade the values and would like to find out two correlated indices that you can trade. In order to select a pair, you need to perform heirarchal clustering and select the one with minimum distance.  
1. Compute returns (percent change) of all indices and store in a variable called returns.  
2. Construct correlation matrix using returns and plot out the correlation plot.  
2. Create heirarchal clustering using returns and plot a dendegram diagram to figure out which two of the indices can be used for pairs trading.  


```R
library(datasets)
head(EuStockMarkets)
```


<table>
<thead><tr><th scope=col>DAX</th><th scope=col>SMI</th><th scope=col>CAC</th><th scope=col>FTSE</th></tr></thead>
<tbody>
	<tr><td>1628.75</td><td>1678.1 </td><td>1772.8 </td><td>2443.6 </td></tr>
	<tr><td>1613.63</td><td>1688.5 </td><td>1750.5 </td><td>2460.2 </td></tr>
	<tr><td>1606.51</td><td>1678.6 </td><td>1718.0 </td><td>2448.2 </td></tr>
	<tr><td>1621.04</td><td>1684.1 </td><td>1708.1 </td><td>2470.4 </td></tr>
	<tr><td>1618.16</td><td>1686.6 </td><td>1723.1 </td><td>2484.7 </td></tr>
	<tr><td>1610.61</td><td>1671.6 </td><td>1714.3 </td><td>2466.8 </td></tr>
</tbody>
</table>




```R

```


```R

```


```R

```

### Good Job! You are done with the section!

## Section 3: Tidymodels

### Question 1 
**The dataset is loaded for you. Perform the following tasks:**  
You have the dataset for rock composition. Using recipe object, perform data pre-processing after splitting the data into train and test. Perform the same steps for both sets of data using the appropriate functions and libraries


```R
head(rock)
```


<table>
<thead><tr><th scope=col>area</th><th scope=col>peri</th><th scope=col>shape</th><th scope=col>perm</th></tr></thead>
<tbody>
	<tr><td>4990     </td><td>2791.90  </td><td>0.0903296</td><td> 6.3     </td></tr>
	<tr><td>7002     </td><td>3892.60  </td><td>0.1486220</td><td> 6.3     </td></tr>
	<tr><td>7558     </td><td>3930.66  </td><td>0.1833120</td><td> 6.3     </td></tr>
	<tr><td>7352     </td><td>3869.32  </td><td>0.1170630</td><td> 6.3     </td></tr>
	<tr><td>7943     </td><td>3948.54  </td><td>0.1224170</td><td>17.1     </td></tr>
	<tr><td>7979     </td><td>4010.15  </td><td>0.1670450</td><td>17.1     </td></tr>
</tbody>
</table>




```R

```


```R

```


```R

```


```R

```

### Good Job! You are done with the section!

## Section 4: Time Series Analysis

### Question 1 
**The dataset is loaded for you. Perform the following tasks:**  
Following is the dataset for quarterly reported earnings (revenues) for JohnsonJohnson.   
1. Parse the data into timeseries format. Create a new variable that is the average of the four columns known as YearEarnings.  
2. Decompose the time series data into trends, seasonal effects, cycles, residuals and plot out the graph for each.  
3. Perform an ARIMA forecast on Qtr1 earnings for the year 1981, 1982.  


```R
print(JohnsonJohnson)
```

          Qtr1  Qtr2  Qtr3  Qtr4
    1960  0.71  0.63  0.85  0.44
    1961  0.61  0.69  0.92  0.55
    1962  0.72  0.77  0.92  0.60
    1963  0.83  0.80  1.00  0.77
    1964  0.92  1.00  1.24  1.00
    1965  1.16  1.30  1.45  1.25
    1966  1.26  1.38  1.86  1.56
    1967  1.53  1.59  1.83  1.86
    1968  1.53  2.07  2.34  2.25
    1969  2.16  2.43  2.70  2.25
    1970  2.79  3.42  3.69  3.60
    1971  3.60  4.32  4.32  4.05
    1972  4.86  5.04  5.04  4.41
    1973  5.58  5.85  6.57  5.31
    1974  6.03  6.39  6.93  5.85
    1975  6.93  7.74  7.83  6.12
    1976  7.74  8.91  8.28  6.84
    1977  9.54 10.26  9.54  8.73
    1978 11.88 12.06 12.15  8.91
    1979 14.04 12.96 14.85  9.99
    1980 16.20 14.67 16.02 11.61
    


```R

```


```R

```


```R

```


```R

```


```R

```


```R

```

## Good Job! You are done with the course!
