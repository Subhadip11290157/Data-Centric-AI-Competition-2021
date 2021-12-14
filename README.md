# How I performed in the Data-Centric-AI-Competition-2021

We were provided with the **_Roman MNIST Dataset_** to filter it for better performance for a given classifier.

<the algorithm(s) used in the model wasn't disclosed to us. Whatever we could manipulate was **ONLY** ~~the~~ **DATA**>

* The contents are specified as under:-

**i>**  **data**:   

>   **Actual or Original**: as we were provided with initially 
  
>   **My Data**: generated images from all sorts of manipulations I performed - automating image cleaning, image augmentation, inverting binary inputs and noise injection to avoid overfitting issues.

**ii>** **third2**:
>   the submission that took me to **133rd** on the leaderboard. 

# Techniques applied on images:- 
> cropping
> rotation (by mild acute angles)
* flipping 
    * (Horizontal - specific to I, II, III, V and X - which are invariant under horizontal flip)
    * (Vertical - specific to I, II, III, and X - which are invariant under vertical flip)
  
> inverse binary thresholding

> dealing with class imbalance issues

> injecting salt and pepper noise (with varying %ages and in seperate customized clusters)

> applying Gaussian blur

> magnification and demagnification

> shearing(along both x and y axes)

> discriminatory distribution of data (intentional) for different labels 
(more training images for conflicting types and less for easily distinguishable ones)

> a bit of heat and trial towards the end with the train vs validation sets' size ratio.
