# Multivariate-QQ-Plot-using-OT
## Overview

This repository provides a function to generate QQ plots and potential plots for multivariate samples. The function is designed specifically for multivariate data and will not work for univariate samples. If your samples are univariate, the methodology coincides with the usual QQ plot.

## Function Usage

qq_and_potential_plots(x, y, p_x, p_y, la=1e-2)

## Parameters:

x: First multivariate sample of length n.

y: Second multivariate sample of length n.

p_x: A vector of size n, where each entry specifies the weight of the corresponding sample point in x. If the samples are i.i.d., all weights should be equal to 1/n.

p_y: A vector of size n, specifying the weights for the y sample.

la: (Optional) A regularization parameter with a default value of 1e-2.

## Returns:

The function returns the QQ plots and potential plots for the provided multivariate samples.

## ⚠ Important Notes

The function only works for multivariate samples. It is not designed for univariate data.

The size of x and y must be the same. A future update will extend support for samples of different lengths.
