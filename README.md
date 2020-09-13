# UnMask: Adversarial Detection and Defense in Deep Learning Through Robust Feature Alignment

### Overview:

To combat adversarial attacks on deep learning models, we developed **UnMask**, 
a knowledge-based adversarial detection and defense framework. 
The core idea behind UnMask is to protect vulnerable deep learning models by verifying that an image's 
predicted class ("bird") contains the expected building blocks (e.g., beak, wings, eyes). 
For example, if an image is classified as "bird", but the extracted building-blocks are 
*wheel*, *seat* and *frame*, we can utilize this information to alert of an potential attack 
and re-classify the image based on it's building blocks. 

![UnMask Framework](images/unmask.jpg)

Extensive evaluation shows that UnMask (1) *detects* up to 96.75% of attacks, with a false positive rate 
of 9.66% and (2) *defends* the model by correctly classifying up to 93% of adversarial images 
produced by the current strongest attack, Projected Gradient Descent, in the gray-box setting.
In addition, UnMask performs 31.18% better than adversarial training when averaged across 
8 attack vectors. Our proposed method is architecture agnostic and fast.

