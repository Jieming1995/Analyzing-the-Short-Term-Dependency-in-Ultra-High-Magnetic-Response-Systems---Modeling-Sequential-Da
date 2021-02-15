# Analyzing the Short-Term Dependency in Ultra-High Magnetic Response Systems - Modeling Sequential Data with Non-Recurrent Neural Networks

Recurrent neural network (RNN) is a popular modeling choice for sequential data. However, empirical experience shows RNNs are often difficult and time-consuming to tune and customize. It drives practitioners to replace RNNs with non-recurrent neural networks which presented comparable performances in some cases. The success of using non-recurrent neural networks to model sequential data indicates the short-term dependency among sequential data. In this paper, we systematically analyze the short-term dependency in ultra-high magnetic response systems (UHMR) with partial system knowledge based on the observability criterion of the dynamic systems. Moreover, we show that the sequential data in the UHMR system only have 2-step dependency. This result indicates that any consecutive three steps in an experiment form a datum to train a feed-forward neural network (FFNN). Therefore, sufficient data can be collected within a small number of experiments. Based on the analysis, we train a feed-forward neural network to model the UHMR system based on the sequential data from four experiments. Through proper data pre-processing, the FFNN model can predict the system performance with bounded mean absolute error. 


# The simulation part of this paper consist of followings: 
## 1. The Euler approximation of UHMR system
This part are included in the "Euler_approxaimation" file.  

## 2. Train FFNN.  
This part is included in File "FFNN".  The trained model is saved in folder "Models" as "FFNN".  

## 3. Train RNN.
We tried three different training datasets in RNN. Check the file "RNN1", "RNN2", "RNN3" for three different training datasets. The RNN training is failed. The final models are saved in folder "Models" as  "RNN1", "RNN2", "RNN3". 
