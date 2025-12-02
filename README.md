# Mitosis Detection Using U-Net

## Overview
This project implements a **Mitosis Detection System** to identify mitotic cells in histopathology images. Using a **U-Net model** with Saliency Maps, the system performs pixel-level segmentation to highlight mitotic areas, aiding in cancer research and medical diagnostics.

---

## Features
- Detects mitotic regions in histopathology images.  
- Uses U-Net for precise pixel-level segmentation.  
- Supports visualization with Saliency Maps to interpret model decisions.  
- Trained and tested on annotated datasets from Roboflow.  

---

## Dataset
- Source: **Roboflow** mitosis detection dataset.  
- Includes annotated images in COCO format for training and testing.  
- Split: `train` and `test` folders containing images and corresponding masks.  

> Add dataset size and number of images if available.

---

## Model / Approach
1. **Data Preprocessing:** Load images and masks, resize and normalize for U-Net input.  
2. **Model Architecture:** U-Net with encoder-decoder structure for segmentation.  
3. **Training:** Train the model on annotated mitotic images using loss functions suitable for segmentation.  
4. **Visualization:** Apply Saliency Maps to highlight mitotic areas and interpret model predictions.  
5. **Evaluation:** Measure performance using metrics like IoU, Dice coefficient, or pixel-wise accuracy.  

---

## Installation
1. Clone the repository:
```bash
git clone https://github.com/PearlAngeline/Mitosis-Detection.git

2. Navigate to the project folder:

cd Mitosis-Detection


3. Install required packages:

pip install -r requirements.txt



## Usage

1. Place the dataset in the respective train and test folders.

2. Train the model:

python train_model.py


3. Predict on test images:

python predict.py --input "test/image_01.png"


4. Visualize predictions with Saliency Maps:

python visualize.py --image "test/image_01.png"


## Results

The model segments mitotic regions accurately in most cases.

Saliency Maps highlight key areas influencing predictions.

Add screenshots of predicted masks and Saliency Maps for better visualization.

## Future Work

Train on larger datasets for improved accuracy.

Experiment with advanced segmentation models (e.g., Attention U-Net, UNet++).

Deploy a web interface for real-time mitosis detection.

## Author

Pearl Angeline – GitHub

## License

This project is licensed under the MIT License – see the LICENSE
 file for details.