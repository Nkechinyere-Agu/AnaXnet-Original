# AnaXnet-Original
The Pytorch implementation of the papaer AnaXnet: Anatomy Aware Chest X-ray findings classification network This implementation requires more memory that the more recent version


![alt text](https://github.com/Nkechinyere-Agu/AnaXNet/blob/master/imgs/network.jpg?raw=true)


### Dependencies
* python 3.5+
* pytorch 1.0+
* torchvision
* numpy
* pandas
* sklearn
* matplotlib
* tensorboardX
* tqdm

### Dataset
Requires MIMIC-CXR Dataset and Chest Imagenome dataset which can both be found on https://physionet.org

to generate the format for object detection from the chest imagenome scene graphs run:
```
python ./data/coco_format.py
```

To train Detectron 2 Faster R-CNN on the coco format dataset, run:
```
python ./detection/objectDetection.py
```

To extract the Anatomical region features from the Faster R-CNN model run:
```
python ./data/featureExtraction.py
```

### Usage
To train a model using default batch size, learning:
```
python train.py  
```

### Results

