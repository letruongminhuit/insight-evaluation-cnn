# Insight Evaluation on Traditional and CNN Features

> Here are our detailed experiments and results we conduted and presented in our current paper with the same name as title. 

### 1. Dataset 
We use two main datasets, namely MNIST and CIFAR-10 with the partitions divided as below:


![image](https://user-images.githubusercontent.com/41055526/131259997-a1450bd1-db64-4c78-9797-5debc9071f6e.png)


### 2. Structures

**Folder: Traditional Filters**

In this folder, we store the code for 14 traditional filters used to extract features from two mentioned datasets: 
1. Prewitt (with X-axis and Y-axis)
2. Sobel filter (with X-axis and Y-axis)
3. Laplacian filter
4. Gaussian Blur filter
5. Local Bimnary Pattern filter
6. Center-Symmetric Local Binary Pattern
7. Spatial Colour Binary Pattern 
8. Multi-channel Local Binary Pattern 
9. Local Ternary Pattern 
10. Completed Local Ternary Pattern 
11. Scale Invarian Local Ternary Pattern 
12. Scale Invariant Center-Symmetric Local Ternary Pattern 
13. Extended Center-Symmetric Local Ternary Pattern
14. Generalized Local Ternary Pattern 

**Folder: CNN Approach**

In this folder, we conducted two practical experiments and store the results evaluated on the test set: 

* Experiment 1: Apply a basic CNN network (14 Conv2D Filters, MaxPooling, Flatten and two FC layers).
* Experiment 2: Apply a basic CNN network as above with additional layers (BatchNormalization and Dropout).

**Files**

* CIFAR - Traditional Filters.ipynb: Store the code for applying traditional filters on CIFAR-10 dataset and create a model prepared for test phase. 
* MNIST-Traditional Filters.ipynb: Store the code for applying traditional filters on MNIST dataset and create a model prepared for test phase.
* Evaluation - CIFAR - Traditional Filters.ipynb: Store the results evaluated on the test set when apply the combination between traditional filters on CIFAR-10 dataset. 
* Evaluation - MNIST - Traditional Filters.ipynb: Store the results evaluated on the test set when apply the combination between traditional filters on MNIST dataset. 

### 3. Architectures for each experiments

##### Traditional Filters

**MNIST Dataset**
Here is the general process how we build model which is combined betwwen diverse traditional filters and start performing ten-class classification task on MNIST dataset:

![image](https://user-images.githubusercontent.com/41055526/131260220-aaf1eedb-eb5d-449b-845e-69a97b40fd5d.png)

**CIFAR-10 Dataset**

Here is the general process how we build model which is combined betwwen diverse traditional filters and start performing ten-class classification task on CIFAR-10 dataset:

![image](https://user-images.githubusercontent.com/41055526/131260239-0938b9f6-124b-4dea-8dc6-d9956a8f8606.png)

##### CNN Filters
Here is the general process how we build model which uses CNN Filters to perform ten-class classification task on both datasets:

![image](https://user-images.githubusercontent.com/41055526/131260267-d6ebedb0-5a9e-44b1-a9b0-09a5b5fa4ef0.png)


### 4. Final results

![image](https://user-images.githubusercontent.com/41055526/131260049-cd70f703-08f0-4bce-afb9-88fff01b18eb.png)

## For further analysis, please refer to the extended version of our paper in the folder `extended-paper`. 

