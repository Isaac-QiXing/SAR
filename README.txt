# SAR
source code of variable selection for spatial autoregssive model

* This package, named SAR, includes the Matlab codes of robust variable selection for
  spatial autoregressive model.

* to run the codes please 

 (1) set the matlab paths by simply  running 
 
 >>  path_setup    
  
 OR 
add the following path manually to the Matlab
path  './',  'lib_m','lib_var','generate_data','Lasso_ISTA'

 (2) run the demo file to test whether the code could run successfully by executing

  >>   demo_spa_reg

 
 It indicates sucessfull runing  if the iterated information and results are printed out: 

....
....
....
the calculated value of rho: 0.6745
spatial regression error: 13.6810
BIC: 559.7777

* folders and functions:

 ./data: consists of the data file of Boston

 ./generate_data: consists of the functions to generate sythetic datasets, and 
    the functions of dealing with the Boston datasets
 
  ./Lasso_ISTA: consisting of the   solvers of ISTA and variable sevelction 
        with  Square Loss + L1 penalty, LAD loss + L1 penalty

  ./lib_m: consists of  the basic functions of general usage (many of them are not used)

  ./lib_var: consists the functions of  robust variable selection, most of the functions of variable 
    selection for SAR model are included in this path 

  
  ./config:  an old  file of parameter settings, please neglect it. 

  ./demo_spa_reg: a  demo file to run robust variable selection by calling ``var_spa_select()''

  ./main_get_data_boston: transform the dataset of Boston for spatial regression
./ main_var_select_boston: main function of variable selection on Boston dataset
./main_var_spa_select: main function of variable selection on the synthetic datasets in the paper
  of   Xijun Liang, etal, Rubust variable selection with exponential squared loss for the spatial autoregressive model.
   CSDA, 2019.

 ./main_putout_elapsed_seconds.m: put out the calculated results of the elapsed seconds
 ./main_putout_result20190806.m: put out the calculated results of ``Correct'', ``Incorrect'', ``rho'', ``MedSE'', etc
./ main_stat_test.m: statistical test of the results by mulitples methods 

./path_setup: function to setup the paths
./readme.txt: this file

* The files could be used freely for your research once you cite the following work

  Xijun Liang, Yunquan Song, Yanji Zhu and Lu Lin, Rubust variable selection with exponential squared 
loss for the spatial autoregressive model. Computational Statistics and Data Analysis, preprint, 2019.

 For commercial usage of this package, please contact    Xijun Liang:  liangxijunsd@163.com

2019.8.28

 
  
