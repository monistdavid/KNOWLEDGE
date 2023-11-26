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

Summary
===============

        
