🛰️ **Semantic Segmentation of Aerial and Multispectral Images**
This project focuses on semantic segmentation of both aerial imagery and multispectral images, leveraging deep learning models to classify each pixel into specific land cover or object categories (e.g., buildings, roads, vegetation, vehicles, etc.).

🔍 **Project Overview**
**Aerial Image Segmentation**
Based on a modified UAVid dataset, aerial images are segmented using a combination of ResNet as the backbone and DeepLabV3 as the segmentation architecture. This setup effectively captures high-level semantic features and fine-grained details, enabling accurate segmentation in complex urban scenes captured from drones.

**Multispectral Image Segmentation**
Using the RIT-18 dataset, which includes images with multiple spectral bands (e.g., NIR, Red Edge), a U-Net architecture was used. The U-Net is customized to handle the additional spectral channels, improving segmentation performance on vegetation and land classification tasks.

🧠**Models Used**
DeepLabV3 + ResNet50 for aerial (UAVid) segmentation

U-Net for multispectral (RIT-18) segmentation

🗂️**Datasets**
**1)Modified UAVid Dataset for aerial imagery**
(High-resolution drone images with pixel-level annotations for urban environments)
Link: https://www.kaggle.com/datasets/giavuongnguyen/modified-uavid-dataset/data

**2) RIT-18 Dataset for multispectral segmentation**
(Includes 6-band multispectral imagery for land cover classification)
Link : https://github.com/rmkemker/RIT-18

⚙️ **Features**
- Custom preprocessing pipelines for RGB and multispectral inputs
- Dataset loading and augmentation
- Visualization of input images, ground truth, and predicted masks
- Evaluation metrics: Mean IoU, Pixel Accuracy, Dice Score
