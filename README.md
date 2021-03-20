

# RDA-Net: Relation-aware Dual-Attention Network for View-invariant Human Action Recognition.

 we propose a Relation-aware Dual-Attention Network (RDA-Net) for  view-invariant action recognition. The RDA-Net is compose of a  relation-aware self-attention module and a  cross-attention module. The  relation-aware self-attention module  learns representative and discriminative features that capture long-range dependencies and pair-wise relationships among human body parts/joints in the spatial and temporal channels. The cross-attention module is designed to learn view-invariant attention maps and generates discriminative features for a semantic representation of actions in different views.
 
 ## Datasets 
 - NTU-60
 - NTU-120
 - UESTC

 ## Attention Results
 
 Here we draw the attention results learned by RDA-Net in NTU-60 dataset, where the radius of the ellipses are proportional to the joint relevance.  The marked greenlight  ellipses  refer  to  the  correct  attention  weights ,  larger radius corresponding to larger weights.
 
![ours_attention](https://user-images.githubusercontent.com/78781422/111570684-4978a700-87e0-11eb-919b-d300b7a53a22.png)
 
 ![attention_58](https://user-images.githubusercontent.com/78781422/111569366-75465d80-87dd-11eb-8159-2154b39f9adf.png)
 
