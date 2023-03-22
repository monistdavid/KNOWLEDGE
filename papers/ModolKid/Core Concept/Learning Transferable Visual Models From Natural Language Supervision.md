Link
===============
<p>

Learning Transferable Visual Models From Natural Language Supervision
https://arxiv.org/pdf/2103.00020.pdf

</p>

Summary
===============
    This paper created Contrastive Language-Image Pre-training (CLIP) that use Contrastive learning method
    to effectively learn the relationship between images and natural languages, instead of single word label. 
    Such a learning gola largely enable the model to understand the latent space of the images and be able to complete
    a lot task without further training (zero shot)


Questions From The Paper
===============


Additional Quesions and Personal Thoughts Based on little RESEARCH
===============
    1. why it is the language model come out first instead of image model, audio model or video model:
        And which of the following has the most information:
        a. text
        b. image
        c. audio
        d. video
        for me from most to least information: d > c > b > a
        Easy to understand the video has the most information as it includes both image and audio, 
        even a little bit text. Compared with audio, the image is not including long sequencing, high dimensional
        data. Carefully thinking, text is a small category of image, it is a pattern composed of lines and shapes as well.
        But still I think image has more information, because it could contains colors, more complex shapes, lines and 
        combinations of all of them. 
    2. natural distribution shifts refer to changes in the distribution of data that are encountered during training 
        and testing processes. One of the most common assumptions in machine learning (ML) is that the training and test
        data are independently and identically distributed, because in real-world scenarios, the data distribution can 
        change over time, and the training data may not fully capture the diversity of the real-world data.
            a. Thinking about this problem, I realized that not only in machine learning, we have similar issues in our 
                daily lives as well. For example, we practice shooting, but in the real game, we can't shot that well. We
                practice math, but in real math exam, we cannot do those questions. We learn knowledge from school, and then
                we realize things are completely different in society. So becoming more successful in the field, we need to
                know what exactly happens in real life scenario, we learn to practice just like we do in real cases. The 
                understanding of the real scenario could help us a lot. How machine learning know the real case? Definitely 
                not from human label, it should from the real data without labeling. 
            b. One of my thoughts for solving this problem the other way is to use the right model to do the right
                thing. In the future, there will be infinitely number of models out there for different data 
                distribution, then try to find the best fit of the model, just like we find the best person for certain 
                things. 
            c. Another method might be, integrate all the models together, so it is a all in one huge model for solving
                all the issues. 
        

Creativity
==============
    1. make a image model that is completely trained with image, none text.
    2. make a auto select system to select the best model for certain task, instead of making one huge model for all
        tasks