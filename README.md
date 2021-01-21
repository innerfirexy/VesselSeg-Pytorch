### __VesselSeg-Pytorch__ : _Retinal vessel segmentation toolkit based on pytorch_
---
### Introduction
This project is a retinal blood vessel segmentation code based on python and pytorch framework, including data preprocessing, model training and testing, visualization, etc. This project is suitable for researchers who study retinal vessel segmentation.

### Requirements  
The main package and version of the python environment are as follows
```
# Name                    Version         
python                    3.7.9                    
pytorch                   1.7.0         
torchvision               0.8.0         
cudatoolkit               10.2.89       
cudnn                     7.6.5           
matplotlib                3.3.2              
numpy                     1.19.2        
opencv                    3.4.2         
pandas                    1.1.3        
pillow                    8.0.1         
scikit-learn              0.23.2          
scipy                     1.5.2           
tensorboardX              2.1        
tqdm                      4.54.1             
```  
The above environment is successful when running the code of the project. In addition, it is well known that pytorch has very good compatibility (version>=1.0). Thus, I suggest you try to use the existing pytorch environment firstly.
### Code structure 

```
└── src
    ├── config.py
    ├── lib
    │   ├── common.py
    │   ├── dataset.py
    │   ├── extract_patches.py
    │   ├── help_functions.py
    │   ├── __init__.py
    │   ├── logger.py
    │   ├── losses
    │   │   ├── __init__.py
    │   │   ├── loss_lab.py
    │   │   ├── loss.py
    │   │   ├── lovasz_loss.py
    │   ├── metrics.py
    │   ├── pre_processing.py
    ├── models
    │   ├── denseunet.py
    │   ├── __init__.py
    │   ├── LadderNet.py
    │   ├── nn
    │   │   ├── attention2.py
    │   │   ├── attention.py
    │   │   ├── deform_conv_v2.py
    │   │   ├── __init__.py
    │   │   ├── new_attention.py
    │   │   ├── sfnet.py
    │   │   └── subpixel_conv.py
    │   └── UNetFamily.py
    ├── prepare_dataset
    │   ├── chasedb1.py
    │   ├── data_path_list
    │   │   ├── CHASEDB1
    │   │   │   ├── test.txt
    │   │   │   └── train.txt
    │   │   ├── DRIVE
    │   │   │   ├── test.txt
    │   │   │   └── train.txt
    │   │   └── STARE
    │   │       ├── test.txt
    │   │       └── train.txt
    │   ├── drive.py
    │   └── stare.py
    ├── test.py
    ├── tools
    │   ├── ablation_plot.py
    │   ├── ablation_plot_with_detail.py
    │   ├── merge_k-flod_plot.py
    │   └── visualization
    │       ├── detail_comparison.py
    │       ├── new_visual.py
    │       ├── preprocess_visualization.py
    │       ├── preprocess_visual_result
    │       └── result_visualization
    └── train.py
```
---
## Quick start 
>### 1) Datasets preparation 
> DRIVE

>### 2) Training model
>Train

>### 3) Test model
>test

## Others 