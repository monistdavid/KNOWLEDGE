Link
===============
<p>

Batch Normalization: Accelerating Deep Network Training by Reducing Internal Covariate Shift
https://arxiv.org/pdf/1502.03167.pdf

</p>

Keyword
===============

    Covariate Shift & Internal Covariate Shift
    Covariate shift is a concept in statistics and machine learning that refers to a situation where the distribution of
    input variables (covariates) in the training data is different from the distribution in the testing or real-world
    application data. This discrepancy can lead to issues when a model trained on one distribution is used to make
    predictions on a different distribution, potentially resulting in poor performance.
    Internal covariate shift refers to the change in the distribution of network activations due to the change in
    network parameters during training. As we know each neural network will be given an input and output, based on 
    the backpropagation, the network will update the parameters. So the distribution of the input will change for each
    layer which will cause the following layers change drmatically, especially the deep layers.

Summary
===============

    This paper introduces a method called batch normalization. The idea is to normalize the input of each layer.
    The normalization is done by using the mean and variance of the batch. Batch Normalization (often abbreviated 
    as BatchNorm) standardizes the inputs to a layer for each mini-batch. This means it normalizes the inputs so that 
    they have a mean of zero and a standard deviation of one. This process is done during training for each mini-batch.
    Usage in a Neural Network:
    Batch Normalization is typically applied after a convolutional or fully connected layer and before a non-linear
    activation function like ReLU.
    
        
