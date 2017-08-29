# GSoC2017
These are the supporting data and documents for OSTSC package.

In GSoC2017, the goal of the project is to develop an R package for imbalance time series data classification. The package has been uploaded to https://github.com/lweicdsor/OSTSC. 

This OSTSC package has been tested on real datasets which are too large to be included in it. The vignettes of OSTSC package displayed three examples, two of them used datasets MHEALTH and HFT, contained in the MHEALTH and toy_HFT folders. The datasets used in the vignettes are pre-processed to form the smaller, more standard datasets for experiments. The R files in the folder is to show how the original datasets be processed.

The other three named 'model saved' folders contain one training result (model, data) in each. 

The python notebook 'Logistic Regression & LSTM Performances Comparison' is a simple example to show how we compared the performances of OSTSC algorithm to other resampling algorithms. We compared with undersampling the majority class, oversampling the minority class, SMOTE and ADASYN. On all the three datasets we used, the OSTSC overperformed others. This notebook is a simple example for how the experiments done. It only run 20 epochs on each LSTM, which is far from converging. So the learning result in it is not accurate.

The core algorithm of OSTSC has already been coded in Matlab, provided by the author. I translated the Matlab codes to R, and completed it to be a package. This package can process multi-class datasets, and has options to apply in parallel. The package has been tested on multiple error input checking and step-by-step data going through comparing between Matlab and R codes. The step-by-step comparison were in the file R v Matlab.

A detailed explanation on how OSTSC performs were stated in the vignettes https://github.com/lweicdsor/OSTSC/blob/master/inst/doc/Over_Sampling_for_Time_Series_Classification.pdf. During the whole project period, I also spent a lot of time on algorithm advantages examination. A concise table of the LSTM learning F1 scores comparison is provided in file LSTM results.


