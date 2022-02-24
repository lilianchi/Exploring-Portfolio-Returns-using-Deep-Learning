### Exploring-Portfolio-Returns-using-Deep-Learning
Try to optimize the sharpe ratio in model 1 and achieve the highest R-aquare in model 2

### Programming language
Python

### Problem 1
Given the 58-year portfolio data, what is the highest sharpe ratio we can achieve?

### Data for Model 1
* data_Z_eff: Feature matrix X with size 2219316×64
* data_R_eff: Cutoff to the output vector with ±0.2 return
* data_R_org_eff Output vector with size 2219316×1
* data_group_ind: starting and ending indices of stocks in time t = 1,2, … , T

### Problem 2
What is the best performance (a.k.a highest R-square) we can achieve with the market return and predictors dataset?

### Data for Model 2
* Xs: A small set of predictors (GoyalWelch) available at the beginning of month t
* Xl: A large set of predictors (GoyalWelch+ Macro variables) available at the beginning of month t
* y: Value-weighted market annual return for month t 

### Paraeters Tuning
* Optimizr: adam, adamax, RMSprop, Learning Rate
* Model structure: #nodes, #layers
* Randomize: LayerNormalization(), BatchNormalization()
* Early stopping: #patience
* Epoch, Batch Size

### Final Result
* sharpe ratio: 9.46
* R-square: -0.287
