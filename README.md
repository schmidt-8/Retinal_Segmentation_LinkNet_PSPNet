# Retinal_Segmentation_LinkNet_PSPNet
Retinal_Segmentation_LinkNet_PSPNet/
├── Data/                              #Folder to store pre-processed data fromall three datasets
├── Datasets/                          #initial folder with only Origa data
├── LinkNetResults/                    #folder for results of LinkNet segmentation
├── NewData/
│   ├── CroppedCenteredData/           #folder for cropped and centered ORIGA data
│   └── Veins/                         #folder for retinal vessels data 
├── NewImages/                         #folder for all unprocessed data from all datasets 
├── NN_notebooks/
│   ├── LinkNet/
│   │   ├── 2_models_combined.ipynb                         #jupyter notebook for LinkNet segmentation of optic cup and disk with combination in the end
│   │   ├── Evaluation.ipynb                                #jupyter notebook for LinkNet models evaluation
│   │   ├── LinklNet_Disk_OneModel.ipynb                    #jupyter notebook for LinkNet optic disk segmentation
│   │   ├── LinkNet_Cup_OneModel.ipynb                      #jupyter notebook for LinkNet optic cup segmentation
│   │   ├── LinkNet_OneModel_MultiChannel_Mask.ipynb        #jupyter notebook for LinkNet segmentation with additional context (3 channel mask)
│   │   ├── LinkNet_Separated_Single_Channel_Masks.ipynb    #jupyter notebook for LinkNet combining two models for segmenting optic disk and cup
│   │   ├── LinkNet_Veins.ipynb                             #jupyter notebook for LinkNet retinal vessels segmentation
│   │   ├── LinkNet_Veins_Loaded.ipynb                      #jupyter notebook for LinkNet to test loading saved models for vessels
│   │   ├── SandBox_Single_mask_segmentation.ipynb          #jupyter notebook for LinkNet development 
│   │   └── Single_Channel_Masks_Disk_Cup.ipynb             #jupyter notebook for LinkNet segmenting optic disk and cup with grayscale input 
│   ├── Preprocessing/
│   │   ├── FolderTool.ipynb                                #notebook for train-test-split and moving images
│   │   ├── Image_augmentation.ipynb                        #notebook fo augmenting cropped images by rotating and flipping them 
│   │   ├── image_convert_dhristi.ipynb                     #notebook for conversion Dhristi data to Origa like data
│   │   ├── image_convert_rimone.ipynb                      #notebook for conversion Rimone data to Origa like data
│   │   ├── Image_crop.ipynb                                #notebook for testing cropping techniques on data
│   │   ├── Image_crop_pipeline.ipynb                       #notebook for automated cropping for whole folder
│   │   └── Image_dilatation.ipynb                          #notebook for creating dilatation masks from ground truth masks
│   ├── PSPNet/
│   │   ├── Evaluation.ipynb                                #notebook for PSPNet model evaluation using IoU, pixel-wise accuracy, dice, confusion matrices
│   │   ├── PSPNet_resnet_Cup.ipynb                         #notebook for PSPNet segmentation of optic cup
│   │   ├── PSPNet_resnet_Disk.ipynb                        #notebook for PSPNet segmentation of optic disk
│   │   ├── PSPNet_resnet_together.ipynb                    #notebook for PSPNet segmentation with additional context (3 channel mask)
│   │   └── PSPNet_sandbox.ipynb                            #notebook for PSPNet development           
│   ├── Combination.ipynb                                   #notebook for combining LinkNet and PSPNet models                                             
│   ├── Evaluation_Combined.ipynb                           #notebook for evaluating LinkNet and PSPNet models         
│   ├── install_torch.txt                                   #folder for pytorch installation with cuda                  
│   └── requirements.txt                                    #dependencies
├── RetinalSegmentation/
│   ├── Images/                                             #folder for desired images to be segmented 
│   ├── Models/                                             #folder for insertion of pretrained models
│   ├── Overlayed_Segmented_Masks/                          #folder for predictions combined with original image
│   ├── Segmented_Masks/                                    #folder for predictions
│   ├── requirements.txt                                    #dependencies
│   └── RetinalSegmentation.ipynb                           #notebook to perform semiautomated segmentation
└── SaveModels/                                             #folder for insertion of pretrained models


