# RDA-Net: Relation-aware Dual-Attention Network for View-invariant Human Action Recognition.

 we propose a Relation-aware Dual-Attention Network (RDA-Net) for  view-invariant action recognition. The RDA-Net is compose of a  relation-aware self-attention module and a  cross-attention module. The  relation-aware self-attention module  learns representative and discriminative features that capture long-range dependencies and pair-wise relationships among human body parts/joints in the spatial and temporal channels. The cross-attention module is designed to learn view-invariant attention maps and generates discriminative features for a semantic representation of actions in different views.

 ## Datasets 
 - NTU-60
 - NTU-120
 - UESTC
 
# NTU RGB+D 60 and 120
-	Request dataset here: http://rose1.ntu.edu.sg/Datasets/actionRecognition.asp
-	Download the skeleton-only datasets:
- Download missing skeletons lookup files from the authors' GitHub repo:

# UESTC-RGB 
-	Request dataset here:  https://github.com/HRI-UESTC/CFM-HRI-RGB-D-action-database

## Training 
- python main.py  – config  ./config/uestc-cross-view/gview_g1.yaml

## Testing 
- python main.py --config ./config/nturgbd-cross-view/evalgview_1.yaml
 


 ## Attention Results
 
 Here we draw the attention results learned by RDA-Net in NTU-60 dataset, where the radius of the ellipses are proportional to the joint relevance.  The marked greenlight  ellipses  refer  to  the  correct  attention  weights ,  larger radius corresponding to larger weights.
 
- RDA-Net Attention weights (camera 1 (45 degree  view).
![RDA_Net_camera_1](https://user-images.githubusercontent.com/78781422/112777576-261de980-9075-11eb-9d4d-1a2fbed29a26.png)

- RDA-Net Attention weights( camera 3 (side view)).
![RDA_Net_camera_3](https://user-images.githubusercontent.com/78781422/112777585-2a4a0700-9075-11eb-82fd-818a94a11429.png)

- RDA-Net Attention weights (Drinking water)
![RDA-Net drinking water](https://user-images.githubusercontent.com/78781422/112777589-2cac6100-9075-11eb-8d16-7b8a2d073dc6.png)

- RDA-Net Attention weights (Hugging other person).
![RDA-Net Hagging](https://user-images.githubusercontent.com/78781422/112777591-2e762480-9075-11eb-87a3-ba51cb49f740.png)

 - RDA-Net Attention weights (Hand-shaking).
 ![RDA-Handshaking](https://user-images.githubusercontent.com/78781422/112778729-b8bf8800-9077-11eb-90c2-a9b57a04ff84.png)
 
 
 # Conclusion 
 In   this   work,   we   have   shown   the   effectiveness   of proposed  relation-aware  self-attention  module  and  cross-attention module in the spatial and temporal channels for view-invariant action recognition.  The relation-aware self-attention module captures local as well as global long-range dependencies of  joints  and  frames  in  the  spatial  and  tempo-ral channels, which learns representative and discriminative features for action representation. The cross-attention module learns co-occurrence attention for action sequences, and minimizes  representation  discrepancy  in  different  views.
 
