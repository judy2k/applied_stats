# Statistics_Module
Creating a project to implement various statistical distributions and methods in Python.

To install and run this project, do the following:
1. Run the following to install: 

``` 
pip install applied-stats
```

2. Follow these examples to start plotting and calculating probabilities. The examples below, and several others, can also be found in the  [Demonstration Jupyter Notebook](https://github.com/WillTirone/applied-stats_examples/blob/main/Demonstration.ipynb)

3. To run the test file, from the command line enter: ```python test.py```

## Usage

### To generate some plots and calculate some probabilities: 

```python
>>> from applied_stats import continuous_distributions
>>> a = Norm_rv(0,1)
>>> a.plot_pdf()
>>> a.probability_calc()
```
![link](https://github.com/WillTirone/applied_stats/blob/main/output_images/N(0%2C1)_plot.png)

```python
>>> q = ChiSq_rv(4,crit_value=7)
>>> q.plot_pdf(cv_probability=True)
>>> q.probability_calc()
```
![link](https://github.com/WillTirone/applied_stats/blob/main/output_images/X-sqr(4).png)

### To calculate the numeric MLE of several common distributions: 

```python 
>>> from stats_tools import mle 
>>> a = [1,3,2,5,6,7,2,3,4,5]
>>> mle.binomial(a)
>>> 3.8

>>> b = [1.2,4.3,2.3,6.8,2.4,3.6]
>>> mle.exponential(b) 
>>> 3.4333333333333336
```
