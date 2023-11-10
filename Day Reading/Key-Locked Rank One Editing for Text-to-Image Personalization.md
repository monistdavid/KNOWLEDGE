Link
===============
<p>

Key-Locked Rank One Editing for Text-to-Image Personalization
https://arxiv.org/pdf/2305.01644.pdf

</p>

Summary
===============
    The new method called Perfusion provides can generate image from text with high fidelity and c
    reativity than Dreambooth.

Questions and Thoughts Based on little RESEARCH
===============
    1. Why overfitting is such a common problem? And why overfitting is such a each behavior?
        Some Personal Thoughts: 
            a. overfitting is common because the models are too eash to tune,
                overfitting is easy because we have a wrong objective when training the model.
            b. overfitting is common because it is easy and overfitting is easy because it is common
        Answer from online:
            Overfitting can happen for various reasons. Sometimes, it occurs when the model is too complex and 
            has too many parameters compared to the amount of training data available. Other times, it happens 
            when the training data is not diverse enough or doesn't represent the full range of possibilities 
            that the model may encounter. Additionally, overfitting can also occur when certain features or 
            patterns in the training data are given too much importance, leading the model to overly rely on them.

Creativity
==============
    1. To improve both of these goals simultaneously, our key insight is that models need to disentangle what 
        is generated from where it is generated.
        a. this is a really interesting thought, the best way to not have the trade-off is to cut the balance bridge