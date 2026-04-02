# ML4P-PS2
Sorry I've only got question 1 done for now, but everything else will be here soon as well.
My even function neural network was EXTREMELY simple, so it ended up doing the simpler function (x**2) pretty well and out performing the baseline, but it did not understand cosine well at all. I compared the baseline to my neural network using root means square error and plots. Here are the RMSE comparisons for both: parabola: baseline RMSE=0.3366, hθ RMSE=0.0379
cosine: baseline RMSE=0.1963, hθ RMSE=0.6647
and the plots are under "cosine_comparison" and parabola_comparison, where hθ is my neural network, the baseline is just the basic sklearn MLPRegressor, and the actual is just the function plotted.
My neural network, hθ, is literally just all of my training data (which was just an array of numbers between -5 and 5) squared, so everything becomes even. This was almost definitely not the most precise way to do this, which is probably why it performed so poorly on cosine.

Sources: https://scikit-learn.org/stable/, https://claude.ai/, https://medium.com/@miosipof/teaching-neural-networks-about-symmetry-673409b28c42, https://numpy.org/doc/2.3/reference/generated/numpy.linspace.html, https://numpy.org/doc/2.2/reference/generated/numpy.ravel.html, https://scikit-learn.org/stable/modules/generated/sklearn.neural_network.MLPRegressor.html 