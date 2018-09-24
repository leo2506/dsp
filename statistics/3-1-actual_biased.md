[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

### Code:
Use the NSFG respondent variable numkdhh to construct the actual distribution for the number of children under 18 in the respondents' households.  
```python
  d = resp.numkdhh
  pmf = thinkstats2.Pmf(d, label='actual')
  pmf
```
#### output:
```
  Pmf({0: 0.466178202276593, 
  1: 0.21405207379301322,
  2: 0.19625801386889966,
  3: 0.08713855815779145,
  4: 0.025644380478869556,
  5: 0.01072877142483318})
```
Now compute the biased distribution we would see if we surveyed the children and asked them how many children under 18 (including themselves) are in their household.  
```python
  biased_pmf = BiasPmf(pmf, label='observed')
  biased_pmf
```
#### output:
```
Pmf({0: 0.0,
1: 0.20899335717935616,
2: 0.38323965252938175,
3: 0.25523760858456823,
4: 0.10015329586101177,
5: 0.052376085845682166})
```
Plot the actual and biased distributions, and compute their means.
```python
  thinkplot.PrePlot(2)
  thinkplot.Pmfs([pmf, biased_pmf])
  thinkplot.Config(xlabel='number of kids', ylabel='PMF')
```
#### output:

![fork](img/forking_repo.png)

  
