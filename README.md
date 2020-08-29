## Title
Image clasification pipeline

## General info
This project contains .ipynb file with show training process for image classification. There are 3 classes: glass, plastic, aluminiun.

## Dataset
Custom dataset which contains images of different bottles (Owner: https://github.com/tapinambur0508)<br>
Train<br>
*aluminium: 642 images
*glass: 369 images
*plastic: 885 images
<br>
Validation<br>
*aluminium: 160 images
*glass: 92 images
*plastic: 221 images
<br>
Test<br>
*aluminium:100 images
*glass:100 images
*plastic:100 images	

## Technologies
Project is created with:
* torch
* torchvision
* opencv
	
## Training Configuration
*batch_size = 25
*epochs_count = 75 
*init_learning_rate = 0.001 
*decay_rate = 0.1  
*num_workers: int = 4  
*device = 'cuda'
*model = pretrained resnet18 with few new layers
*metric = accuracy
*loss func = weighted cross entropy

## Performance
*training loss: 0.01246
*training accuracy: 0.995
*validation loss: 0.00535
*validation accuracy: 0.99577
*training time: 4080.65s
*test accuracy: 0.997 (299/300)
*one image on CPU < 0.2s
![Example of using model](https://github.com/Zhovtukhin/Bottles-Clasification/sample_prediction.png)
![Confusion matrix for test images](https://github.com/Zhovtukhin/Bottles-Clasification/performance.png)"# Bottles-Clasification" 
