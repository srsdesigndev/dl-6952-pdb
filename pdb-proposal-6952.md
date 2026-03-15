**Health by the Numbers: Predicting Diabetes and BMI with Deep Learning**  
*Course Project Proposal*  
Dataset: CDC Diabetes Health Indicators | Source: UC Irvine Machine Learning Repository  
URL: https://archive.ics.uci.edu/dataset/891/cdc+diabetes+health+indicators  
   
**Research Questions**  
**RQ1 (Classification)**  
   
Can we predict if a patient has diabetes or not based on lifestyle factors like BMI, blood pressure, cholesterol levels, and physical activity?  
**RQ2 (Regression)**  
Can we predict a patients BMI based on lifestyle factors like age, income, physical activity, general health rating, and smoking habits?  
**Step 1: Framing the Problem and Looking at the Big Picture**  
**How would the answers to your RQs be useful or beneficial to other people?**  
The answers to the classification RQ would be useful to other people because if it is possible to predict if a patient has diabetes or not, it will really help doctors and nurses to identify patients who may be on the verge of having diabetes. The answers to the regression RQ would be useful to other people because if it is possible to predict a patients BMI, it would really help to identify the lifestyle factors associated with a patients BMI. Both RQs are quite relevant to real-life situations.  
**For the classification RQ, are you more interested in precision, recall, or F1 score?**  
   
The most important of these is recall. If the model fails to detect someone who has diabetes, it is much worse than if it detects someone who doesn’t. A false negative could mean the person doesn’t receive treatment on time, which could have serious repercussions on the person’s health. A false positive just means the person must go through a few extra tests, which isn’t ideal but is much less damaging. So, we need to maximize the recall even if it means sacrificing some precision.  
**For the classification RQ, propose two models and one baseline model.**  
The baseline model will be Logistic Regression since it’s a simple and easy to interpret model that is commonly used in medical research for binary classification tasks. The first main model will be a basic feedforward Neural Network with one hidden layer using ReLU activations, which is a good starting point for tabular data like this. The second model will be a deeper Neural Network with two or more hidden layers and dropout added in to help prevent overfitting.  
**For the regression RQ, propose two models and one baseline model.**  
The baseline model would be Linear Regression because it is the most basic model to use when trying to predict a continuous value. The first model would be a Feedforward Neural Network with a single hidden layer and a linear output layer to deal with the regression problem. The second model would be a deeper version of the previous model with batch normalization and dropout layers to improve how well it generalizes to data it has not seen during training.  
**Name at least 3 major hyperparameters you plan to tune.**  
The learning rate is perhaps one of the most important hyperparameters because it controls how fast the model learns, and if it is set incorrectly, it can take an eternity to train. The number of hidden layers is also very important because it determines how complex the model is, which is essential to how well it learns to recognize patterns. The dropout rate is also a hyperparameter we want to optimize because it helps prevent the model from memorizing data. The batch size is another hyperparameter we want to optimize, which determines how stable the training process is.  
**Step 2: Get the Data**  
**Where did you obtain the dataset?**  
This dataset was retrieved from the UC Irvine Machine Learning Repository, which is an approved source for this assignment. The data is publicly accessible and can be downloaded from the site.  
**Does this dataset appear to have missing data?**  
No, since it is already a clean version of the original data from the CDC’s Behavioral Risk Factor Surveillance System Survey.  
**What types of data are in this dataset?**  
The data is a tabular data stored in a CSV file containing different types of data: numerical data such as BMI and days with poor physical and mental health, categorical data such as smoking status and high blood pressure status, and ordinal data such as rating of general health, age groups, income levels, and education levels.  
**How many instances and features are in this dataset?**  
   
There are 253,680 instances and 22 features in total: 21 features and 1 target variable, which is diabetes status. This is already far more than the 750 instances and 10 features required by the assignment. If the data is too large to be used for model training, we can use random sampling to reduce the size of the data to a more manageable size.  
**How does this dataset allow you to answer your two research questions?**  
For the classification problem, the target is the Diabetes binary column, which is 0 if a patient does not have diabetes and 1 if a patient has prediabetes or diabetes. The other 21 features are used as inputs to the model. In the regression problem, we will change things up a bit. In this problem, BMI will be used as a target, and the other 20 features will be used as inputs. These two questions are using the same set of data and have the same theme, which is health and lifestyle and how it relates to diabetes.  
