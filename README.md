# CS302-Python-2020-Group39

### Dataset:
For access to our data-set, click on the Kaggle link and press the download tab:
https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia

***

### Instructions for training particular models:

**AlexNet**: on line 175, change model to equal model = AlexNet().to(device) <br>
**LeNet5**: on line 175, change model to equal model = LeNet5().to(device) <br>
**VGG-16**: on line 175, change model to equal model = vgg16().to(device) <br>
**ResNet50**: on line 175, change model to equal model = ResNet50().to(device) <br>

***

### Instructions on loading the dataset: 

- on the lines 159 and 163 attach the file location path for trainset and testset:
- trainset = torchvision.datasets.ImageFolder(root='./data/chest_xray/train', transform=transform)
- testset = torchvision.datasets.ImageFolder(root='./data/chest_xray/test', transform=transform)

### Results
AlexNet produced the best results out of the 4 models. It’s final epoch returns an accuracy of 86%. Both ResNet50 and LeNet5 had similar results of 82% and 81% respectively. VGG16 had the lowest accuracy of 76%.
***
![](/images/11.PNG)
***
![](/images/12.PNG)
![](/images/13.PNG)
