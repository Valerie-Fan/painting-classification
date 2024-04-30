# painting-classification
The notebook demonstrates how to use the YOLOv5 model for painting classification, focusing on the setup, dataset preparation, and model training.

## Dataset:
The notebook uses a custom dataset likely fetched from Roboflow, as indicated by the code. Detailed information about the dataset source (wikiart-v4) is utilized.

## Model:
The model employed is YOLOv5, a popular model for object detection tasks, adapted here for classifying paintings.

## Requirements:
- Python 3.x
- PyTorch
- Requirements listed in `requirements.txt` of the YOLOv5 repository

## Setup Instructions:
1. Clone the YOLOv5 repository and install dependencies:
   ```bash
   git clone https://github.com/ultralytics/yolov5
   cd yolov5
   pip install -qr requirements.txt
   ```

2. Ensure the directory structure is correct for downloading the dataset:
   ```bash
   mkdir -p ../datasets
   cd ../datasets
   ```

3. Run the training script from the YOLOv5 directory:
   ```bash
   cd ../yolov5
   python classify/train.py --model yolov5s-cls.pt --data $DATASET_NAME --epochs 100 --img 128 --pretrained weights/yolov5s-cls.pt
   ```

## How to Run:
Open the notebook in a Jupyter environment and execute the cells sequentially, following the instructions within each cell.