Link
===============
<p>

A Simple Framework for Contrastive Learning of Visual Representations
https://arxiv.org/pdf/2002.05709.pdf
https://github.com/google-research/simclr


</p>

Understand the question
===============

    Contrastive Learning
    Contrastive learning is a technique in machine learning, particularly in the field of unsupervised learning, 
    where the model learns to distinguish between similar (positive) and dissimilar (negative) pairs of data points.
    It's often used in scenarios where labeled data is scarce or unavailable. 

Questions and Thoughts Based on little RESEARCH
===============

    1. why nonlinear transformations are also crucial, and what is the relationship between activation function
        and nonlinear transformation?
        1. all activation functions are nonlinear transformations, not all nonlinear transformations are activation 
            functions. Activation functions are a specific tool used within the broader scope of nonlinear 
            transformations in neural networks. So adding a nonlinear transformation at the end is similar to adding a 
            activation function (Just a different way to call it)
    2. Training with large batch size may be unstable when using standard SGD/Momentum with linear learning rate 
        scaling (Goyal et al., 2017). To stabilize the training, we use the LARS optimizer.
        1. typically the learning rate is scaled linearly with the batch size. However, this might cause the model to 
        be in the local optimum. So we use LARS optimizer to stabilize the training. In the LARS optimizer, we 
        have different learning rate for different layers. It scales the learning rate based on the ratio of
        the weight norms to gradient norms for each layer.
    3. small weight and large weight in the model:
        a "weight" refers to a parameter within the network that determines the strength of the influence one neuron 
        has on another. The weight is adjusted during training based on the loss function and backpropagation. If a 
        single weight is too large, it means cerain features is over amplified, which will make the model overspe
        -cialize on that single feature. The reason why a single weight has that much influence is the neuron's weight
        might have a lot more influence on its further layers. so that we have the weight decay method to control such
        problem.
        weight decay
        Benefits:
        Prevents Overfitting: By penalizing large weights, weight decay reduces the model's tendency to fit noise 
        in the training data.
        Improves Generalization: Models regularized with weight decay often perform better on unseen data, as they 
        tend to learn more general patterns.
        Stability in Optimization: Adding weight decay can also stabilize the training process, especially when 
        using large learning rates.

Summary
===============

    1. it is not all true that all the features should be generalized. Some features should be specialized. 
        For example, a human always has similar shape, body, arms, heads, etc. Weight decay method completely ignore
        the cases that certain features could be specialized.
        
