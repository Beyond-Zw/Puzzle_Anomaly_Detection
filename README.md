# Puzzle-AE: Novelty Detection In Images Through Solving Puzzles

<img src="Images/Method.png" alt="hi" class="inline"/>

### 1- Clone this repo:
``` bash
git clone https://github.com/Niousha12/Puzzle_Anomaly_Detection.git
cd Puzzle_Anomaly_Detection
```
### 2- Datsets:
This repository performs Novelty/Anomaly Detection in following datasets: MNIST, Fashion-MNIST, CIFAR-10, COIL-100, MVTec AD, and 2 medical datasets (Head CT (hemorrhage) and Brain MRI Images for Brain Tumor Detection).

Datasets MNIST, Fashion-MNIST, CIFAR-10, and COIL-100 will be downloaded by Torchvision. You have to download [MVTec AD](https://www.mvtec.com/company/research/datasets/mvtec-ad/), [Head CT (hemorrhage)](https://drive.google.com/drive/folders/1AO2Vd29e6N1eC6dqT8OKYy7QwFa19xsu?usp=sharing), and [Brain MRI Images for Brain Tumor Detection](https://drive.google.com/drive/folders/1c2YkU3uAfAcmdbkdIKdg6veftXyMmOmE?usp=sharing), and unpack them into the `data` folder.

### 3- Checkpoints:

### 4- Train the model:
Start the training using the following command. The checkpoints will be saved in the folder `checkpoints`.
``` bash
python train.py --config configs/config_train.yaml
```

### 5- Test the trained model:

