# An analysis of the multi-armed bandit strategy for web service optimization

As Github renderer is not always working well, here is the [HTML version](http://htmlpreview.github.io/?https://github.com/gdonval/AB_testing_MultiArmedBandit/blob/master/html/AB_testing_MultiArmedBandit.html).

In recent years, people working in the interweb figured out that they could actually make decisions based on actual data.
Thanks to advanced behavior tracking and and basic statistical analysis,
they are able to grasp a little bit of a *hidden truth* about people to "optimize" their service accordingly.

However, sound statistics often require setups considered less-than-optimal from a business standpoints. 
For instance, A/B testing requires that you serve each particular version of your website evenly over user
for the whole duration of the test, even though a peek in the data shows that one version is clearly yielding
better results.
That is why more or less efficient strategies were devised to "improve" upon A/B testing.

The purpose of this notebook is to analyze one of these strategies based on the multi-armed bandit setup.
