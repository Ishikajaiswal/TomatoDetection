# Tomato Detection
Model to classify and detect ripe and raw tomatoes.

------
## Scripts
- [TomatoDetection_Preprocessing.ipynb](https://github.com/Ishikajaiswal/TomatoDetection/blob/main/TomatoDetection_Preprocessing.ipynb)
    - Extracts labels and images for training an RCNN from the [dataset](https://www.kaggle.com/andrewmvd/tomato-detection)
- **Training Scripts**: The ResNet50 model is trained on the dataset using pre-trained ImageNet weights
    - [TomatoDetection_Train1.ipynb](https://github.com/Ishikajaiswal/TomatoDetection/blob/main/TomatoDetection_Train1.ipynb)
    - [TomatoDetection_Train2.ipynb](https://github.com/Ishikajaiswal/TomatoDetection/blob/main/TomatoDetection_Train2.ipynb)
    - [TomatoDetection_Train3.ipynb](https://github.com/Ishikajaiswal/TomatoDetection/blob/main/TomatoDetection_Train3.ipynb)
- [TomatoDetectionandClassification.ipynb](https://github.com/Ishikajaiswal/TomatoDetection/blob/main/TomatoDetectionandClassification.ipynb)
    - This script uses our trained model to detect and classify ripe and raw images. 
    - The ROI (Region Of Interest) is detected using selective search in OpenCV. 
    - These ROIs are then fed into the model for classification. 
    - All the overlaps are detected and deleted using IoU (Intersection over Union) and other methods.
    - The final bounding boxes are then classified into ripe and raw tomato images using color filters in OpenCV.
------
## Work to be done
- Improve the ROI detector to detect less number of and more accurate ROIs.
- Enhance the color filter to detect red tomatoes more accurately.
- Train the model on more data so that it generalises better.
------
The link to the trained models can be found [here](https://drive.google.com/drive/folders/1bPs3VRbccQDOEulMbJSXyenPapvSAejb?usp=sharing)
