# semantic-segmentation-of-satellite-imagery

This code implements a semantic segmentation model for aerial imagery using a U-Net architecture. It utilizes the TensorFlow and segmentation_models libraries. The dataset (https://www.kaggle.com/datasets/humansintheloop/semantic-segmentation-of-aerial-imagery) consists of labeled aerial images with six classes: Building, Land (unpaved area), Road, Vegetation, Water, and Unlabeled. The code preprocesses the data by patchifying both the images and their corresponding labels. 

The U-Net model is defined with a contracting and expansive path, employing convolutional layers with batch normalization, dropout, and max-pooling. The Dice loss function is used for optimization, and metrics such as accuracy and Jaccard coefficient are employed for evaluation. The final trained model is evaluated on a test set, and the Jaccard coefficient (Intersection over Union) is calculated to assess the segmentation performance. The model gets an IoU of greater than 0.7.

![image](https://github.com/Rhugved-Kale/semantic-segmentation-of-satellite-imagery/assets/86423298/68e57e60-b174-4318-860f-39c5cb4b71f2)
