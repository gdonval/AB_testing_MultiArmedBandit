# An analysis of the multi-armed bandit strategy for web service optimization

*As Github Jupyter notebook renderer is not always working well, here is the [HTML version](http://htmlpreview.github.io/?https://github.com/gdonval/AB_testing_MultiArmedBandit/blob/master/html/AB_testing_MultiArmedBandit.html).*

In recent years, people working in the interweb figured out that they could make decisions based on actual data from their existing user base.
So they devised advanced behavior tracking and statistical analysis frameworks to "optimize" their service accordingly.

Most of these frameworks tend to use statistically sound one-size-fits-all approaches such as A/B testing and some multivariate analysis derived from it. These methods are rigorously correct, powerful and require a great amount of bad luck and incompetence to really go wrong.

However that rigor can be considered less-than-optimal from a business standpoints: while you spend time assessing which button color yields the highest click-through rate, you do not benefit from the results obtained until then. Nothing is worst than having a peek in the data, to figure out that one version performs a lot better than the others (double meaning, I know).

That's why new methods were created to arguably perform "better" than A/B testing. Some do in specific cases and fail miserably in others without a warning. Most skew the data in so subtle ways that nobody ever figures out that their 99% significance level is actually closer to 40%. And so on.

The multi-armed bandit strategy is one of such "superior" method and has been adapted to web optimization: this is what we study in this notebook.
