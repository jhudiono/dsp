[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

    resp = nsfg.ReadFemResp()
    actual_pmf = thinkstats2.Pmf(resp.numkdhh, label='actual')
    biased_pmf = BiasPmf(actual_pmf, label='biased')
    thinkplot.Pmfs([actual_pmf, biased_pmf])
    thinkplot.Config(xlabel='number of children', ylabel='PMF')
    print('Actual mean', actual_pmf.Mean())
    # Actual mean 1.024205155043831
    print('Biased mean', biased_pmf.Mean())
    # Biased mean 2.403679100664282`
