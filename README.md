# Semantic segmentation and anomaly detection on roads
Segmentation Problem Computer Vision

Author: Miguel Fernández Lara

## Project Structure

### main.ipynb

The complete project is inside the main notebook. The structure is the following:


main.ipynb
```text
│
├─ 1. Project Setting
│
├─ 2. Setup
│
├─ 3. Dataset Loading and Exploration
│
├─ 4. Data Augmentation and Loaders
│
├─ 5. Semantic Segmentation (Closed-Set)
│ ├─ 5.1 Baseline: Naive Majority Class Segmentator
│ ├─ 5.2 FCN + ResNet50
│ ├─ 5.3 FCN + ResNet50 + Focal Loss
│ ├─ 5.4 U-Net
│ ├─ 5.5 DeepLabV3+
│ ├─ 5.6 SegFormer
│
├─ 6. Anomaly Exploration
│
├─ 7. Anomaly Detection
│ ├─ 7.1 Testing the Models
│ │ ├─ 7.1.1 FCN + ResNet50
│ │ ├─ 7.1.2 U-Net
│ │ ├─ 7.1.3 DeepLabV3+
│ │ └─ 7.1.4 SegFormer
│ └─ 7.2 Qualitative Analysis (anomaly heatmaps)
│
├─ 8. Ablation Study
│ ├─ 8.1 Global Segmentation Performance (mIoU)
│ └─ 8.2 Anomaly Detection Ablation (AUPR / AP)
│
└─ 9. Final Conclusion
```

### Model weights

A folder "models" is provided with the ".pt" files of the several models weights.
Due to the size of the folder, a One Drive link is provided:
https://liveunibo-my.sharepoint.com/:f:/g/personal/miguel_fernandezlara_studio_unibo_it/IgCfo1rYFlpvTrOB-A-QWHxkAZ8pcTqMEtHy8KFnB61GmQI?e=CMXQUa


## Instructions to Run the Notebook

The notebook has been turned in with all cells run and plots displayed. However, it can be run if needed.
This project is designed to be run on **Google Colab**, using a **GPU runtime**.

### Running Instructions (Colab)

1. Open the notebook(s) in **Google Colab**

2. Enable GPU:
   - `Runtime: Change runtime type: GPU`

3. Download the model weights from the link and upload the ".pt" files to a Google Drive folder 

4. Inside the main.ipynb, in the project settings sections, configure the correct paths.

5. Mount Google Drive with the code provided

6. Ensure the dataset and model paths are correctly set to the correct ones in your directory

7. Set the flag: training = False (to skip training and only run evaluation)

8. Run all cells sequentially from top to bottom

Average run-all time: 1 hour 15 minutes (mIoU computations are heavy)
If GPU time is over, change google accounts or buy computation units and proceed with the run all
