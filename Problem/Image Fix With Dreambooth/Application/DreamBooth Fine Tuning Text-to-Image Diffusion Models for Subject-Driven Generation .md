Link
===============
<p>

DreamBooth: Fine Tuning Text-to-Image Diffusion Models for Subject-Driven Generation
https://arxiv.org/pdf/2208.12242.pdf

</p>

Summary
===============
    This paper proposed a method on finetune the text-to-image generative model like stable diffusion. 
    By using a unique identifier and a class prior perservation training method to prevent language drift, 
    reducing output diversity problem to help better finetune the text-to-image generation model in order
    to maintain high fidelity of the model and high diversity of the context at the same time.


Questions and Thoughts Based on little RESEARCH
===============
    1. Author mentioned the language drift and reduced output diversity issue in the paper: 
        in general, they have the same concept, when we want the model to especially do certain task better, 
        they forget how to do the other tasks. Thinking about when human learn, we won't completely forget to do other
        tasks when we learn a specific new task, or let's say the phenomeno is not that obviously. Why is that?
        a. Besides language itself, we have a lot other factors that influence our learning process. We are allowed
            to talk with people using learned language even we are learning different language.
        b. We know we learn those language not for our daily life communication but for something else
    2. 


Creativity
==============
    1. why, where, when, how, what, when a language model learn the task, make a world learning model as a huge 
        context. 