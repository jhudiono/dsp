[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)


    # [177.8 cm, 185.42 cm]
    lower = thinkstats2.EvalNormalCdf(177.8, mu, sigma)
    upper = thinkstats2.EvalNormalCdf(185.42, mu, sigma)
    print("{0:.0%}".format(upper - lower))
>> 34%
