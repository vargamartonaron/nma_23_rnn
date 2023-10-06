# Project repository to the Neuromatch Academy Computational Neuroscience course
## Brief description of the RNN model
### This project revolves around a Recurrent Neural Network (RNN) that has been trained to output neural activity. It has the input of a value between 1-20 which is converted into a one-hot encoding which is fed into the network. The output simulates neural activity of individual neurons. 
## Task outline
### Our task was two-fold. First, we needed to find a way to benchmark the model. Second, we wanted to make biologically plausible implementations into our provided RNN model that emulates the process of working memory in the human brain. 
## Task 1
### We created a simple neural network with 1 hidden layer and 140 neurons with a ReLu activation function. A combination of these three seemed to work the best for benchmarking. The reasoning behind using this method as a benchmarking technique was that we could test the efficacy of our RNN by seeing how many iterations it would take for our decoder to predict the input into the model at a >95% accuracy. By doing this, we could see how well the initial information was retained throughout the network. 
## Task 2
### In order to make our RNN model more biologically plausible, we inserted an excitatory and inhibitory component into our synaptic weights that aligned with the proportions that has been observed in the brain. Our stated hypothesis was that there would be a fine balance between excitation and inhibition where the efficacy RNN model would be optimized when the two components were equal. If excitation is too intense in relation to inhibition, then the network will perish. If inhibition is disproportionately large, then the network will fail as well.
## FINDINGS
### Excessive excitation is much worse than excessive inhibition for network efficacy
### By meddling with tau (the time step for the RNN network), we serendipitously discovered that if tau > 6ms our decoder performed much better when it came to predicting previous inputs of the model. We believe that the previous inputs resonated for longer in the system. If tau < 6ms then the decoder performed much better at predicting recent inputs into the RNN model.
## Conclusion
### All in all, this project was a great exploration that taught all of us a geeat deal about how to interact with and analyze neural networks. Despite not having been able to make any concrete conclusions about the differences between RNN and working memory in humans due to severe limitations in the biological complexity of the initial RNN model, we left this project feeling fulfilled and prepared for the next neural network project that lands at our feet.
