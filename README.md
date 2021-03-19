# EmberData
Data used for Ember Projects

This contains the data used for the examples in the paper
Daly, C. An application of an Embedded Model Estimator to a synthetic non-stationary reservoir model with multiple secondary variables 
Front. Artif. Intell. | doi: 10.3389/frai.2021.624697

It consists of a directory of 4 files, split with Winzip. The files are
1) SmoothFew
2) SmoothMore
3) SmoothMany
4) SmoothAll

The first 3 consist of training data sets of varying amounts of spatial data, while the 4th has a set of target variables where a trained model should be applied.
The data is in GSLIB format
In the paper, the target variable is PorosityTrueSmooth and the model is trained on all variables except FaciesSmooth and channelonly. 

The code used in the paper is owned by Schlumberger Limited and, currently, is only available commercially. It is based on an extension of Random Forest suitable for spatial interpolation and stochastic simulation. The idea is to make Random Forest Spatially aware by 'embedding' spatial estimators. In the paper, the embedded estimater is Kriging. 

The theory is described in a bit more detail in 
Daly. C An Embedded Model Estimator for Non-Stationary Random Functions using Multiple Secondary Variables https://arxiv.org/abs/2011.04116 (to appear in Math Geosci)
