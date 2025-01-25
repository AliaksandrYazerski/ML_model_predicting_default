# ML_model_predicting_default
**Project objective:** To create a model for predicting the risk of a client's default on a loan.

Default is the failure to pay interest on a loan or bonds, failure to repay a loan within a certain period of time t. Usually, a default is considered to have occurred if the client has not made a loan payment within 90 days.

This model allows a bank or other credit institution to assess the current risk for any issued loans and credit products and, with a greater degree of probability, prevent the client from failing to fulfill their credit obligations. Thus, the bank is less likely to incur losses.

### Project objectives:
1. Select Features from the source data.
2. Predict default (estimated ROC-AUC value ~ 0.75).
3. Pack the resulting model into an automated PipeLine, which, when fit() is called, will prepare the data and train the model, and when predict() is called, will make predictions on a given data set (1 - fact of default).

### Initial data:
1. Files "train_data_#.pq" with description of data about clients.
2. File "train_target.csv" with completed events (there was a fact of going to default/no).

### Main stages of work on the project:
1. Load initial data from parquet files.
2. Prepare initial data and select features.
3. Select, train and evaluate the quality of models.
4. Wrapping the process of creating the best model in PipeLine.
5. Train PipeLine on the entire dataset and save the training result in binary рiскlе format.