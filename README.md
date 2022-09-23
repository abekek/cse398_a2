# CSE 398/498. Assignment 2
#### Student Name: Alibek Kaliyev
#### Email: alk224@lehigh.edu

## Installation
1. Create an environment from ```environment.yml``` file:
```
conda env create -f environment.yml
```

2. Activate the environment:
```
conda activate cse398_alk224
```

3. Verify that the environment was installed correctly:
```
conda env list
```

## Usage
Each of the following commands should be run from the ```src/``` directory of the project. Run the following command in your terminal to move there:
```
cd src
```

### Task 1
To run the task 1, run the following command:
```
python task1.py
```

Wait for the program to finish running. The output will be saved in the ```output/``` directory. After the image is displayed, press ```Enter```on your keyboard to move further.

### Task 2
To run the task 2, run the following command:

```
python task2.py
```

Wait for the program to finish running. The output will be saved in the ```output/``` directory. After the image is displayed, press ```Enter```on your keyboard to move further.

### Task 3
To run the task 3, run the following command:

```
python task3.py
```

Wait for the program to finish running. The output will be saved in the ```output/``` directory. After the image is displayed, press ```Enter```on your keyboard to move further.

#### Explanation for Task 3

For this task I did not use any morphological operations, since the provided image was initially good for extracting features, i.e. none of the objects had holes in them, or were touching each other. I used the Otsu's thresholding to binarize the image, similarly as in task1 and task2.

As a feature to extract, I used maximum axis length because oval objects have longer axis than round ones. Then I figured out the threshold of 40 from the histogram of the feature values. At the end, I used the threshold to separate the objects into two groups: round and oval.