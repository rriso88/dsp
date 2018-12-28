[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

x = np.random.random(1000)  
# PMF is a function that gives the probability that   
# a discrete random variable is exactly equal to some value  
pmf = thinkstats2.Pmf(x)  
thinkplot.Pmf(pmf, linewidth = 0.1)  
thinkplot.Config(xlabel = 'Random', ylabel = 'PMF')  
