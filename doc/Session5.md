# Session 5: Cloud Computing

## Teachable Machine from Google
Today we are going to learn some interesting tools about ***"AI on the cloud"***.

We will explore the fun features of Google's teachable machine, and then further combine it with our SenseStorm.

Nevigate to Teachable machine's [page](https://teachablemachine.withgoogle.com/) and explore the three categories. 
- image classification
- audio classification
- pose estimation

## Hyperparameters for your training
There will be several hyperparameters during your training process.

### Epochs
Epochs stands for how many times your sample data have been gone through by your model.

The larger the epochs, the longer the trainning time may it cosumes.

### Batch Size
Your data will be split into several batches to feed your model. Batch size stands for how large would each batch be.

### Learning Rate
The learning rate may be the most important hyperparameter when configuring your neural network. Therefore it is vital to know how to investigate the effects of the learning rate on model performance and to build an intuition about the dynamics of the learning rate on model behavior.

## Export your models onto SenseStorm
After playing around with Teachable Machine, we need to implement the models on SenseStorm.

The python script is already on this repository, but you need to have it installed on SenseStorm:
```
cd Desktop
git clone https://github.com/VanpleW/SKSS
```

Go to the folder: TeachableMachine and use TM2_tflite.py to implement your trained model.
```
cd SKSS/TeachableMachine
```

You need to transfer your downloaded files from your laptop to SenseStorm via ***WinSCP***.

### File Transfer Option 1: WinSCP
First you need to download and install the WinSCP at [Ninite](https://ninite.com)

Type your SenseStorm IP as the host IP, and input the SenseStorm username and password to login.

![WinSCP](winSCP.png)

Then you could drag your downloaded files from your laptop to SenseStorm. Remember your destination path should be TeachableMachine in this SKSS directory.

### File Transfer Option 2: Cloud Drive
You could use Google Drive, Dropbox etc to upload files from PC and download them from SenseStorm.

### File Transfer Option 3: USB Flash Dirve
You could also copy files with your USB flash drive.

## MNIST experiment on Colab
After learning the simplest the cloud-based AI training, we are now going to learn something more practical. We will try a MNIST experiment on another Google Cloud Computing Platform: [Colab Notebook](https://colab.research.google.com/notebooks/intro.ipynb#recent=true).

Please follow the instruction of Dr. Zhang and copy the codes [Here](https://raw.githubusercontent.com/yzhang0301/codes/master/mnist.py) into your colab environment.

Then we are going to use the cloud GPU machine to execute the codes.