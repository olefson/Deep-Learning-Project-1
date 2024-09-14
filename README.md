# Deep-Learning-Project-1
A simple 5 layer deep neural network using Python and TensorFlow

Homework 2 
 
1. (50 pts) Setup Python and Tensorflow and implement a deep neural network with 5 
layers. Use the first three column of the provided data to predict the third column label.  
Randomly select 90% of the data for training and test on the rest 10% of the data. You 
can use any Python and Tensorflow library.  
 
Your submission should include  
- neural network training source code (30 pts) 
- a test script that can load the trained neural network and run it on the test dataset (10 
pts) 
- a figure of validation loss for each epoch and test loss for each epoch (10 pts) 
 
2. (50 pts)  
- Provide results with and without normalization (standard scaling) (10 pts) 
- Provide results with two different mini-batch sizes (5 pts) 
- Provide results with two different learning rates (5 pts) 
- Provide results with Momentum and Adam optimizer (5 pts) 
- Provide results with two different initialization approaches: random and Xavier (10 pts) 
- Provide results with and without regularization (5 pts) 
Provide the code with all the options (commenting out one option) 
Provide all results as figures

Project Description:
Determine if a baby is in pain or not based of its vitals

Dataset:
5 Columns 
1. Index
2. Heartrate of baby
3. Respiratory Rate of baby
4. Oxygen Saturation Level
5. Is baby in pain or not (0, 1, 2, or #)
    0: baby is not in pain
    1: mild pain
    2: strong pain
    #: label is missing (label not collected)

Submission:
2 files:
1. Training Code
2. Testing Code

Notes: 

After first test run, there is a problem with getting stuck at 56.6% accuracy. This is confermed to be because of a significant class imbalance in the dataset (severe pain is underrepresented)
Attempted fix: use class weights to assign higher weights to underrepresented classes during the model's training step. The goal being to penalzie misclassifications in minority classes more heavily, encouraging the model to pay more attention to them. 