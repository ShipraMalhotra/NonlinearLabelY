# Non linear Label Y

**Original Publication**: Song J. Bias corrections for Random Forest in regression using residual rotation. *Journal of the Korean Statistical Society*. **2015** 44 (2015) 321–326.

This paper talks about weighted tree predictionis but for classification tasks. The script here has been modified to work for regression tasks.

Same as the authors, we use the simulation data (Breiman, 2001) from the following model:

    f (x) = 10sin(πx1x2) + 20(x3 − 0.5)2 + 10x4 + 5x5 + ϵ,

where ϵ follows the normal distribution with mean zero and standard deviation σ and xi are uniformly distributed between 0 and 1 for i = 1, 2, . . . , 10. The input variables x5, . . . , x10 are the noise variables that are irrelevant to the response variable. We generate the sample of size 1000 for the training set and 1000 for the test set.

The authors analysed the performance of their model with changing the standard deviation σ from 1, 5, 10. 

- σ  = 1 : NonlinearY.ipynb
- σ  = 5 : NonlinearY_sd_5.ipynb
- σ  = 10 : NonlinearY_sd_10.ipynb
