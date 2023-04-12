Link
===============
<p>

Pre-train, Prompt, and Predict: A Systematic Survey of Prompting Methods in Natural Language Processing
https://arxiv.org/pdf/2107.13586.pdf

</p>

Summary
===============

Questions and Thoughts Based on little RESEARCH
===============
    1. The order of the AI model:
        Fully supervised learning -> Neural Network 
        -> Pre-trained & Fine-tuned -> Prompt
        -----------------------------
        featured based -> automatically feature generation 
        -> decrease dataset requirement -> template based task completion
        -----------------------------
        what's next?
        As I mentioned before, language/text is a type of image, is it possible to generate the text as an image?
        The book "Story Of your life" describing this woman scientist studying allen's language and she found that 
        there is not an order of writing the allen language. Or it is not right to say write the language, but more 
        like drawing the language. Human being can only write the language lines by lines because it is easier to 
        comprehend and digest. Things are really weird that human being should be able to understand the images
        much faster than reading language. Then why do we read language instead of putting all the information in the 
        images and digest images directly. 
    2. fine-tuning is hard for the trillion-scale models. 
        From ChatGPT:
                Firstly, the large size of these models requires a significant amount of computational resources, 
            such as high-end GPUs or TPUs, to perform fine-tuning efficiently.
                Secondly, the massive number of parameters in these models can lead to overfitting if not 
            appropriately regularized during fine-tuning. This can lead to poor generalization performance
            on new data.
                Thirdly, the dataset used for fine-tuning may need to be appropriately preprocessed to handle 
            the sheer volume of data. This can include techniques such as data sharding, data batching, and 
            distributed training to make the fine-tuning process feasible.
                Finally, tuning the hyperparameters of these large models can also be a challenging task. 
            Given the sheer number of hyperparameters to tune, it can be difficult to find an optimal set of
            hyperparameters that leads to the best performance.
        
        



Creativity
==============
    1. Making a model that instead of writing a paragraph, draw a paragraph from random direction. 