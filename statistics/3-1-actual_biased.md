[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

### Code:
Use the NSFG respondent variable numkdhh to construct the actual distribution for the number of children under 18 in the respondents' households.  
```python
  d = resp.numkdhh
  pmf = thinkstats2.Pmf(d, label='actual')
  pmf
```

  
