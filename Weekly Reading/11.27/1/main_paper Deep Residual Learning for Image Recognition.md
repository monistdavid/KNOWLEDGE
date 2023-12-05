Link
===============
<p>

Deep Residual Learning for Image Recognition
https://arxiv.org/pdf/1512.03385.pdf
https://www.youtube.com/watch?v=GWt6Fu05voI
https://www.youtube.com/watch?v=kYB8IZa5AuE

</p>

Understand the question
===============

    Deep Residual Learning

    Deep Residual Learning is a method for training very deep neural networks, and it was introduced to address the
    degradation problem commonly encountered in these networks. The key idea behind Deep Residual Learning is the use of
    residual blocks or residual functions. Let's break down this concept for better understanding:

Questions and Thoughts Based on little RESEARCH
===============

    1. By using the identity mapping, we could make sure at least the deeper network could perform the same as the 
        shallower network. Then why there will be a degradation problem?
        firstly, identity mapping is hard to train as well. 
    2. why transforming input x to a same dimension as F(x) will not influence the info from x?
        because it is under a linear transformation. The property of linear transformation is:
            1. all lines remain lines
            2. the origin remains fixed 
    3. We also notice that the deeper ResNet has smaller magnitudes of responses
        the residual function is calculating the differnce between the desired output and input, an identity mapping
        is just the 0 of the output of this function. So based on the identity mapping, the function tends to give
        small magnitudes of responses.
        


Summary
===============

        
