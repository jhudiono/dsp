[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

    nums = np.random.random(1000)
    pmf = thinkstats2.Pmf(nums)
    thinkplot.Pmfs([pmf])
    thinkplot.Config(xlabel='number', ylabel='PMF')
>> Each number should be equally likely (0.1%) if it is random.

    cdf = thinkstats2.Cdf(nums)
    thinkplot.Cdfs([cdf])
    thinkplot.Config(xlabel='number', ylabel='CDF')
>> Linear so uniform distribution.
