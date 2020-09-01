# Puzzle-AE: Novelty Detection In Images Through Solving Puzzles

This repository contains code for training and evaluating the proposed method in our paper [Puzzle-AE: Novelty Detection in Images through Solving Puzzles](https://arxiv.org/pdf/2008.12959.pdf).

<img src="Images/Method.png" alt="hi" class="inline"/>

### 1- Clone this repo:
``` bash
git clone https://github.com/Niousha12/Puzzle_Anomaly_Detection.git
cd Puzzle_Anomaly_Detection
```
### 2- Datsets:
This repository performs Novelty/Anomaly Detection in the following datasets: MNIST, Fashion-MNIST, CIFAR-10, COIL-100, MVTec AD, and 2 medical datasets (Head CT (hemorrhage) and Brain MRI Images for Brain Tumor Detection).

Datasets MNIST, Fashion-MNIST, CIFAR-10, and COIL-100 will be downloaded by Torchvision. You have to download [MVTec AD](https://www.mvtec.com/company/research/datasets/mvtec-ad/), [Head CT (hemorrhage)](http://www.kaggle.com/felipekitamura/head-ct-hemorrhage), and [Brain MRI Images for Brain Tumor Detection](http://www.kaggle.com/navoneel/brain-mri-images-for-brain-tumor-detection), and unpack them into the `Dataset` folder.


### 3- Train the Model:
Start the training using the following command. The checkpoints will be saved in the folder `outputs/{dataset_name}/{normal_class}/checkpoints`.

Train parameters such as dataset_name, normal_class, batch_size and etc. can be specified in `configs/config_train.yaml`.
``` bash
python train.py --config configs/config_train.yaml
```

### 4- Test the Trained Model:
Test parameters can be specified in `configs/config_test.yaml`.
``` bash
python test.py --config configs/config_test.yaml
```
