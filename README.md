# ML_IDCard_Segmentation (IN WORK)
Machine Learning Project to identify an ID Card on an image.

## Additional Information
Dataset: [MIDV-500](https://arxiv.org/abs/1807.05786)   
Tensorflow Version: GPU 1.5.0

## Installation
1. Create and activate a new environment.
```
conda create -n idcard python=3.6
source activate idcard
```
2. Install Dependencies.
```
pip install -r requirements.txt
```

## Download and Prepare Dataset
Download the image files (image and ground_truth).  
Splits the data into training, test and validation data.
```
python prepare_dataset.py
```

### Training of the neural network
```
python train.py
```

### Test the trained model
```
python test.py
```

### Additional commands
Starts Tensorboard Visualisation.
```
tensorboard --logdir=logs/
```

## Background Information

### Metrics
The metric used is the [Dice Coefficient (F1 Score)](https://arxiv.org/pdf/1606.04797v1.pdf).
![Dice F1 Scpore](assets/dice.png "Dice F1 Scpore")

