Link
===============
<p>

Learning Transferable Visual Models From Natural Language Supervision
https://arxiv.org/pdf/2103.00020.pdf

</p>

Summary
===============
<p>

Learning Transferable Visual Models From Natural Language Supervision
https://arxiv.org/pdf/2103.00020.pdf

Contrastive Representation Learning: A Framework and Review
https://arxiv.org/ftp/arxiv/papers/2010/2010.05113.pdf

</p>

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
            Thinking about this problem, I realized that not only in machine learning, we have similar issues in our 
            daily lives as well. For example, we practice shooting, but in the real game, we can't shot that well. We
            practice math, but in real math exam, we cannot do those questions. We learn knowledge from school, and then
            we realize things are completely different in society. So becoming more successful in the field, we need to
            know what exactly happens in real life scenario, we learn to practice just like we do in real cases. The 
            understanding of the real scenario could help us a lot. How machine learning know the real case? Definitely 
            not from human label, it should from the real data without labeling. 
        

Creativity
==============
    1. make a image model that is completely trained with image, none text.