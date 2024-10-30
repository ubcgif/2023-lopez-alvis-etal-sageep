# A convolutional neural network for the classification of UXO in  marine settings

_Jorge Lopez-Alvis, Lindsey J. Heagy, Douglas W. Oldenburg, Stephen Billings and Lin-Ping Song_

![thumbnail](./abstract/thumbnail.png)

## Summary 

Multicomponent time-domain electromagnetic (TDEM) systems have been successfully used to detect and classify unexploded ordnance objects (UXOs) in terrestrial settings. Typically, classification uses features derived from a physics-based inversion process which assumes a dipolar response and recovers the principal axis polarizabilities of an object. The recovered polarizabilities are then compared with a library of known ordnance objects and a class is assigned. In marine settings, several complicating factors are introduced. Firstly, the conductive seawater and sediments have an EM response that can significantly obscure target responses. Secondly, there is a much larger uncertainty in sensor positioning as compared to the terrestrial case. These factors may adversely impact inversion results and hence classification. Machine learning (ML) methods, and in particular convolutional neural networks (CNNs), have been successful in classifying directly from data given a sufficiently large set of labeled examples. Our work is examining the use of CNNs to classify ordnance objects from TDEM data. We have implemented a CNN that preserves both spatial and temporal information across layers by considering 3D convolutions (two spatial dimensions and one temporal dimension). We attained fine resolution classification by considering spatially distributed outputs, which is analogous to an image segmentation problem. Once trained, our CNN outputs a probability that the signal in a given receiver position is associated with an ordnance object. Training of the CNN was done with synthetic data generated using ordnance libraries by randomly assigning class, noise level and location and orientation of the target object. Our initial focus is on terrestrial data to develop a proof-of-concept for the use of CNNs as a complementary tool to inversion-based classification of UXO from TDEM data. Preliminary results for a field test plot show that our CNN approach is able to detect all shallow targets and correctly classify 65% while the remaining 35% are classified as UXO but the type is misclassified. The CNN classification produces a rate of about 20% false detections (i.e. labeling as a target of interest where none is present). In order to improve CNN-based classification accuracy, we are currently investigating new network architectures and input features. Finally, we plan to test the CNN with marine data and, if needed, make further changes so that it is robust to the particular challenges of seawater response and higher positional uncertainty.

## Citation 



