# Churn-Prediction-Using-KNIME-Tool

### Churn prediction:
Churn prediction modelling techniques attempt to understand the precise customer behaviours and attributes which signal the risk and timing of customer churn. Churn prediction is the use of statistics and data about your customers to try to model who might leave for another service. Customer churn, also known as customer attrition, occurs when customers stop doing business with a company. The companies are interested in identifying segments of these customers because the price for acquiring a new customer is usually higher than retaining the old one.

### What is KNIME Analytics Platform?
KNIME Analytics Platform is the free, open-source software for creating data science. It is helping you discover the potential hidden in your data, mine for fresh insights, or predict new features.

### Build Our First Workflow in KNIME
Let’s say that we have some Bank Customers data that we want to process, analyze and visualize. With the following example workflow, we will read, transform and visualize this BankCustomers.csv data.

![1](https://user-images.githubusercontent.com/80674012/116277310-f7458100-a7a2-11eb-9e60-270dc96cf647.png)

### Build Customer Churn Prediction Model in KNIME
Step 1 – Download data from our GitHub account and create new workflow
To get started, first download the BankCustomers.CSV file that contains the data that you are going to use in the workflow. Open your Analytics Platform and create a new, empty workflow by clicking “New” in the toolbar.
![2](https://user-images.githubusercontent.com/80674012/116278042-b4d07400-a7a3-11eb-95f6-e2e67763c3a3.png)

Step 2 – Drag and drop CSV file into workbench editor
From the download folder, drag and drop the CSV-file into the workbench editor.

Step 3 – Statistics Node, Statistics view of the Bank Customers.
To Visualize some of the columns, by using the Statistics node.


Step 4– Number to String Node
To Convert Exited column in to String, by using the Number to String node.

Step 5– Color Manager Node, Color By Churn
To set Color by Churn, by using the Color Manager Node.

Step 6–Histogram Node, Count Exited or Not Exited Bank Customers
To Visualize the Histogram and count the value of Exited Bank Customer=1 and Not Exited Bank Customer= 0, by using the Histogram Node.

Step 7– Pie/Donut Chart Node, Customer’s Geography
To Visualize the Pie Chart and count the Customer’s Geography by using the Pie/Donut Chart Node.


Step 8– Partitioning Node, Split Data into Train & Test
For building a Machine Learning Algorithm we always need train and evaluate (Testing) data. For this reason, the Partitioning node is required to partition most of the data (80%) for training and the small remaining amount (20%) for evaluation (Testing).


Step 9– Decision Tree Learner Node,
Train Decision Tree Model


Step 10– Decision Tree Predictor
Model Evaluation:


Step 11– Scorer Node, Check the Accuracy Score & Confusion Metrix
For Check the Model Accuracy Score and Confusion Metrix by using the Scorer Node.


Step 12–PMML Writer Node
Save the model in .PMML file

Deployment
When we are satisfied with our model performance, we can move it into production for deployment on real data. Here we need only read the stream of real-life data coming in through a file or database or whatever other data source and the generated model. We then apply a Decision Tree Predictor, a PMML Predictor to run the model on the real-life input data. The output data will contain a few additional columns with the prediction class and the probability distributions for both classes churn=0 and churn=1, if so specified in the predictor configuration settings.


Step 13 – Drag and drop New Data file into workbench editor
Drag and drop the new data TestBankCustomer.xlsx into the workbench editor. Excel Reader node will appear on the workflow editor and its configuration dialog will pop-up.

Step 14–PMML Reader Node, Load the model 
For Load the Predicted Model using the PMML Reader Node.


Step 15–PMML Predictor Node
Predict customer will Exit bank or not that’s way we use PMML predictor Node.

Step 16–Data To Report Node
View the predicted report of customer will Exit bank or not that’s way we use this Node.

### These Blog and KNIME Workflow is available on our GitHub.
### Blog Site:     
### GitHub Link:	 
https://github.com/SMIIT-Projects/Churn-Prediction-Using-KNIME-Tool

### Tools and Technologies:
KNIME 4.3.2 (64bit)


## Thank You!


