Link
===============
<p>

Neural Codec Language Models are Zero-Shot Text to Speech Synthesizers
https://arxiv.org/pdf/2208.12242.pdf

</p>

Summary
===============
        This paper purposed a pre-trained method of zero-shot text to speech. It referenced the idea of GPT-3, pairing 
    the phonme transcription and audio sample of a dataset with 60K hours (hundred times bigger than any other dataset).
    It could convert the audio with transcript to a discrete acoustic tokens (codes), then use decoder to reconstruct
    it back. As it is trained on a huge audio/transcript dataset, it is able to applied on different speakers and be 
    able to store speakers' information like emotions as well.
        It is the first text-to-speech model that used the language model approach and significantly outperforms the
    previous zero-shot text-to-speech methods. 



Questions and Thoughts Based on little RESEARCH
===============
    1. if we believe a smarter student could learn things faster, why a large language model could not learn domain 
        knowledge fast? Could not be fine-tuned easily? 
            By saying easily, we should mean it learns faster and better with a relatively small dataset. It actually takes
        a much larger computational cost. So by focusing on a spcefic task, but relatively easy task, there is no need to 
        use extremely large language models. Smaller models like GPT-J should be good enough. 


Creativity
==============
