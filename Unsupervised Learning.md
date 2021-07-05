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

## Good Job! You are done with the course!
