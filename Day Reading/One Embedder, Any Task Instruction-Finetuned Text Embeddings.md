Link
===============
<p>

One Embedder, Any Task: Instruction-Finetuned Text Embeddings
https://arxiv.org/pdf/2212.09741.pdf

</p>

Summary
===============
        This paper use contrastive learning and instruction based embedding method to further improve
    the performance of the text embeddings on semantic similarity task. 

Questions and Thoughts Based on little RESEARCH
===============
    1. we were only able to use four negative examples during the model 
        finetuning process due to computation constraints. However, negative examples have been shown
        to play an important role in contrastive learning (Robinson et al., 2021). 
        a. Is the usage number of negative number higher the better? And why?

Creativity
==============
    1. However, most existing embeddings can have significantly degraded performance when applied to 
        new tasks or domains.
        a. Is it possible to apply different embeddings for the same text for different people?
    2. For asymmetric tasks such as retrieval, where the input is a single sentence query and the
        output is a document, the instructions reflect that difference.
        a. Seems like more features are using to make the model stronger. The problem is how to make
            model use more features. Unsurpervised learning make the model extract features by themselves.
            What else could human being help in this case? 