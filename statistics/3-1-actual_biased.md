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
  Pmf({0: 0.466178202276593, 1: 0.21405207379301322, 2: 0.19625801386889966, 3: 0.08713855815779145, 4: 0.025644380478869556, 5: 0.01072877142483318})
```

  
