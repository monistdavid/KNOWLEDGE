Link
===============
<p>

You Only Look Once: Unified, Real-Time Object Detection
https://arxiv.org/pdf/1506.02640.pdf

</p>

Understand the question
===============

    Object Detection
        Determining the location of one or more objects in an image and drawing abounding box around their extent.
        Assigning a class label to each object identified in the image (e.g., cat, dog, car, etc.).
        Object detection is to locate the position and identity of one or more objects in an image.

Questions and Thoughts Based on little RESEARCH
===============

    1. Why author choose to use a unified architecture and try to solve the problem as a regression problem?
        1. simplify to question (there are couple complex process in the traditional method like region proposal, 
            feature extraction, classification, and bounding box regression), the unified architecture try to solve 
            them all in one time, I guess the reason is because the dataset is large enough and the model structure
            is complex and advanced enough to solve all the question at the same time.
        2. It depends on the purpose of the model. YOLO tries to do the object detection as quickly as possible, a 
            unified architecture is needed in this scenario, the problem left is to guarantee the accuracy as well as 
            the speed.
        3. End to end system is good for global image and effortless manual engineering but it's difficult to train 
            such a model because of several reasons.
    2. By watching the video of YOLO:  https://www.youtube.com/watch?v=MPU2HistivI
        Pros:
            1. it is really fast
        Cons:
            1. it is bad on small object detection
            2. when objects are moving, it is hard to do the object detection
            3. the localization is not accurate on small object
        Question:
            Can it guess what is hidden by certain object?
                YOLO normally only infer the visible part
    3. Because the YOLO see the global context, it makes much less mistakes on differentiate the background image. 
        Besides see the whole image during the training, is there any other way to decrease the background image 
        mistakes numbers?
        1. does contrastive learning help decreasing the mistakes? By using the background image as negative examples
            and foreground image as positive examples. maybe it could decrease the mistakes of recognizing the 
            background as image.
        2. If the contrastive learning on background helps improving the performance of the model. Does the contrastive
            on object detection itself help? For example, use dog as a postive exmaple for dog, cat then as a negative
            example. 
    4. pros and cons of IOU, any alternatives?
        Pros: 
            1. simple and intuition
            2. balanced measurement method
        Cons:
            1. it doesn't give the error a weight, when the  IOU have some small error, it just says the error is big
                or small based on the math, however, some of the objects might be a lot different even though their
                IOU is similar
        GIOU, DIOU, CIOU: Generalized IOU (GIOU), Distance IOU (DIOU), and Complete IOU (CIOU) 
    5. For each of the bounding box we try to detect the object, we calculate the  class-specific confidence scores 
        for each box. Do they all have the same weight?
        1. it seems like given certain component more weight will give the model a better performance
            in certain task. For example, if more weight on (Pr(Classi | Object)), then it does better at 
            making accurate prediction; however, it might be bad on localization.
    6. convolutional layer and fully connected layer
        convolutional layer: extract and generalize features, preserving spatial relationships
        fully connected layers: classifiers
    7. extensive data augmentation
        Extensive data augmentation refers to the process of applying a wide range of transformations to the 
        training data to create new and varied examples.
    8. solution for imbalanced data:
        in general: Undersampling methods eliminate the majority class instances in the data to make the data more 
                    balanced. 
                    In oversampling, the goal is to increase the count of minority class instances to match it with 
                    the count of actual majority class instances.
        can pretraing on model could help reducing the imbalanced data problem when training a new model


Summary
===============


Creativity
==============
        