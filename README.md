# Neural_Network_Charity_Analysis

## Project Overview
Alphabet Soup, a non-profit, has requested assistance determining whether or not an organization will be successful if funded by Alphabet Soup for a project. Specifically, the non-profit requested assistance in creating a binary classifier that can predict success rates. Additionally, a neural network model will be designed. Data for over 34,000 organizations will be used for this project. The first step for this project is to preprocess the data for a neural network model. The second step is to compile, train, and evaluate the model. The third and final step is to optimize the model. The goal of the model is to have a predictive accuracy higher than 75% for whether or not the organization will be successful if funded. 


## Resources
- Data: charity_data.csv
- Python 3.7.13, Pandas, Scikit-Learn, TensorFlow Library


## Results

### Deliverable 1: Preprocessing Data for a Neural Network Model

The first step was to preprocess the data using Pandas and Scikit Learn. 

Data Preprocessing: 
- The target variable for this binary classification model is the "IS_SUCCESSFUL."
- The featured variables for this model are "STATUS", "ASK_AMT", "IS_SUCCESSFUL", "APPLICATION_TYPE_Other", "APPLICATION_TYPE_T10", "APPLICATION_TYPE_T19", and "APPLICATION_TYPE_T3." 
- The "EIN" and "NAME" variables were removed as they are purely identification variables and not target or feature variables. 

Merged DataFrame:

<img width="1102" alt="Screen Shot 2022-09-04 at 12 58 27 PM" src="https://user-images.githubusercontent.com/103774401/188327385-0a16973b-0ffb-4cd5-94d0-708111a0d37a.png">

### Deliverable 2: Compile, Train, and Evaluate the Model

A neural network model to create a binary classification model was created. The model indicates whether or not the funded organizations will be successful.

<img width="832" alt="Screen Shot 2022-09-04 at 2 38 57 PM" src="https://user-images.githubusercontent.com/103774401/188331097-d525e858-8262-4579-af44-afe6cf1835fb.png">

### Deliverable 3: Optimize the Model
The model was then optimized in an attempt to achieve an accuracy of higher than 75%. 

Compiling, Training, and Evaluating the Model:
- The number of neurons originally selected was 75 and 25 since this dataset has a high number of values. Two layers were created and the relu activation function was used for those layers. For the output layer, sigmoid activation was used. 
- The target model performance of a predictive accuracy higher than 75% was not achieved. 
- Four attempts were made to optimize the model. The first attempt to optimize the model was by increasing the neurons from 75 to 125 and 25 to 75, the second attempt involved increasing the epochs from 100 to 150, the third attempt involved adding a third hidden layer with 10 neurons, and the fourth attempt involved combining the three prior attempts (a third hidden layer was added, the epochs were increased, and the neurons were increased. 

Attempt 1: Increasing Neurons

<img width="914" alt="Screen Shot 2022-09-04 at 2 45 58 PM" src="https://user-images.githubusercontent.com/103774401/188331109-4340dd4b-edcd-474a-8967-5aef7f43a60e.png">

Attempt 2: Increasing Epochs

<img width="1034" alt="Screen Shot 2022-09-04 at 2 45 13 PM" src="https://user-images.githubusercontent.com/103774401/188331102-b51b5f94-608f-41c2-892d-548bc5d0f652.png">

Attempt 3: Adding a third hidden layer

<img width="1028" alt="Screen Shot 2022-09-04 at 2 53 02 PM" src="https://user-images.githubusercontent.com/103774401/188331139-b8fff6ea-85f9-44fc-97b3-336b50f80189.png">

Attempt 4: Increase neurons, increase epochs, and add a hidden layer

<img width="1130" alt="Screen Shot 2022-09-04 at 2 50 00 PM" src="https://user-images.githubusercontent.com/103774401/188331118-ab008ef4-5a55-438b-a50a-b162079ea304.png">

## Summary
The data was successfully preprocessed and a binary classification model. Even though several attempts were made to reach an accuracy of higher than 75%, the model was not able to do this. The accuracy for the original model was 0.7259 (72.59%), the accuracy for the first attempt to optimize the model was 0.7244 (72.44 %), the accuracy for the second attempt was 0.7268 (72.68 %), the accuracy for the third attempt was 0.7261 (72.61%), and the accuracy for the fourth attempt was 0.7257 (72.57%). The highest accuracy was when the the epochs were increased. This model could be optimized further by increasing the epochs. However, a different model may be better to classify the organizations. A random forest classifier model would be optimal for this project as random forest models typically have high accuracy, which is the issue with the binary classification model in this project. 
