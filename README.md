# Retinal_Segmentation_LinkNet_PSPNet
This repository contains source codes to all implementation done in this diplom thesis. 
Tu successfuly test image segmentation follow these steps:

1) Download repository content as .zip file
2) Download pretrained models from https://drive.google.com/file/d/1QGT-qbTl1OLmH7JKAWEK9YUdeTQhtw9S/view?usp=sharing
3) Unzip both .zip files
4) Extract RetinalSegmentation folder
5) Install virtual enviroment in this folder
6) Install all dependncies in requirements.txt
7) Move content from downloaded models from google drive to the RetinalSegmentation/Models according to README in RetinalSegmentation/Models.
8) Open RetinalSegmentation.ipynb and run all cells
9) Check your final results in Overlayed_Segmented_Masks and Segmented_Masks folders.

   
```
Retinal_Segmentation_LinkNet_PSPNet/                                                                                                                              
├── Data/                              # Folder to store pre-processed data from all three datasets                                     
├── Datasets/                          # Initial folder with only Origa data
├── LinkNetResults/                    # Folder for results of LinkNet segmentation
├── NewData/
│   ├── CroppedCenteredData/           # Folder for cropped and centered ORIGA data
│   └── Veins/                         # Folder for retinal vessels data
├── NewImages/                         # Folder for all unprocessed data from all datasets 
├── NN_notebooks/
│   ├── LinkNet/
│   │   ├── 2_models_combined.ipynb                         # Jupyter notebook for LinkNet segmentation of optic cup and disk with combination in the end
│   │   ├── Evaluation.ipynb                                # Jupyter notebook for LinkNet models evaluation
│   │   ├── LinklNet_Disk_OneModel.ipynb                    # Jupyter notebook for LinkNet optic disk segmentation
│   │   ├── LinkNet_Cup_OneModel.ipynb                      # Jupyter notebook for LinkNet optic cup segmentation
│   │   ├── LinkNet_OneModel_MultiChannel_Mask.ipynb        # Jupyter notebook for LinkNet segmentation with additional context (3 channel mask)
│   │   ├── LinkNet_Separated_Single_Channel_Masks.ipynb    # Jupyter notebook for LinkNet combining two models for segmenting optic disk and cup
│   │   ├── LinkNet_Veins.ipynb                             # Jupyter notebook for LinkNet retinal vessels segmentation
│   │   ├── LinkNet_Veins_Loaded.ipynb                      # Jupyter notebook for LinkNet to test loading saved models for vessels
│   │   ├── SandBox_Single_mask_segmentation.ipynb          # Jupyter notebook for LinkNet development 
│   │   └── Single_Channel_Masks_Disk_Cup.ipynb             # Jupyter notebook for LinkNet segmenting optic disk and cup with grayscale input 
│   ├── Preprocessing/
│   │   ├── FolderTool.ipynb                                # Notebook for train-test-split and moving images
│   │   ├── Image_augmentation.ipynb                        # Notebook for augmenting cropped images by rotating and flipping them 
│   │   ├── image_convert_dhristi.ipynb                     # Notebook for conversion Dhristi data to Origa like data
│   │   ├── image_convert_rimone.ipynb                      # Notebook for conversion Rimone data to Origa like data
│   │   ├── Image_crop.ipynb                                # Notebook for testing cropping techniques on data
│   │   ├── Image_crop_pipeline.ipynb                       # Notebook for automated cropping for whole folder
│   │   └── Image_dilatation.ipynb                          # Notebook for creating dilatation masks from ground truth masks
│   ├── PSPNet/
│   │   ├── Evaluation.ipynb                                # Notebook for PSPNet model evaluation using IoU, pixel-wise accuracy, dice, confusion matrices
│   │   ├── PSPNet_resnet_Cup.ipynb                         # Notebook for PSPNet segmentation of optic cup
│   │   ├── PSPNet_resnet_Disk.ipynb                        # Notebook for PSPNet segmentation of optic disk
│   │   ├── PSPNet_resnet_together.ipynb                    # Notebook for PSPNet segmentation with additional context (3 channel mask)
│   │   └── PSPNet_sandbox.ipynb                            # Notebook for PSPNet development           
│   ├── Combination.ipynb                                   # Notebook for combining LinkNet and PSPNet models                                             
│   ├── Evaluation_Combined.ipynb                           # Notebook for evaluating LinkNet and PSPNet models         
│   ├── install_torch.txt                                   # Folder for PyTorch installation with CUDA                  
│   └── requirements.txt                                    # Dependencies
├── RetinalSegmentation/
│   ├── Images/                                             # Folder for desired images to be segmented 
│   ├── Models/                                             # Folder for insertion of pretrained models
│   ├── Overlayed_Segmented_Masks/                          # Folder for predictions combined with original image
│   ├── Segmented_Masks/                                    # Folder for predictions
│   ├── requirements.txt                                    # Dependencies
│   └── RetinalSegmentation.ipynb                           # Notebook to perform semiautomated segmentation
└── SaveModels/    
```
