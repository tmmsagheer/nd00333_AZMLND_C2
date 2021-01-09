# Operationlising ML Pipeline

In this project, we do the following:
1. Create an Auto ML experiment
2. Deploy the best Auto ML experiment ranked on Accuracy as a REST endpoint that could be communicated with HTTP
3. Repeat the same with Azure Python SDK using the Jupyter Notebook provided above

## Architectural Diagram
![Architecture](https://github.com/tmmsagheer/nd00333_AZMLND_C2/blob/master/starter_files/Images/Architecture.png)


## Key Steps
1. Upload Bank Marketing Dataset from: https://automlsamplenotebookdata.blob.core.windows.net/automl-sample-notebook-data/bankmarketing_train.csv
![Registered Dataset](https://github.com/tmmsagheer/nd00333_AZMLND_C2/blob/master/starter_files/Images/Registered_Datasets.png)
2. Create an Automated Machine Learning Experiment and Execute the same
![Completed AML Experiment](https://github.com/tmmsagheer/nd00333_AZMLND_C2/blob/master/starter_files/Images/Completed_AML.png)
3. The best model graded on our choice metric (Accuracy in this project) is shown besides the status of the Experiment.
![Best Model](https://github.com/tmmsagheer/nd00333_AZMLND_C2/blob/master/starter_files/Images/Completed_AML2.png)
![Best Model](https://github.com/tmmsagheer/nd00333_AZMLND_C2/blob/master/starter_files/Images/BestRunModel2.png)
![Best Model](https://github.com/tmmsagheer/nd00333_AZMLND_C2/blob/master/starter_files/Images/BestRunModel.png)
4. Deploy the best model, eable authentication and wait for REST endpoint and SWAGGER URI creation
![Deploy Model](https://github.com/tmmsagheer/nd00333_AZMLND_C2/blob/master/starter_files/Images/DeployModel.png)
5. Enable Application Insights using logs.py script.
![Endpoint Logging](https://github.com/tmmsagheer/nd00333_AZMLND_C2/blob/master/starter_files/Images/logs1.png)
![Endpoint Logging](https://github.com/tmmsagheer/nd00333_AZMLND_C2/blob/master/starter_files/Images/logs2.png)
6. Run Swagger on locahost and serve a python HTTP server on localhost
![swagger Documentation](https://github.com/tmmsagheer/nd00333_AZMLND_C2/blob/master/starter_files/Images/swagger1.png)
![swagger Documentation](https://github.com/tmmsagheer/nd00333_AZMLND_C2/blob/master/starter_files/Images/swagger2.png)
7. Consume the deployed model using HTTP by means of the endpoint.py script. The REST endpoint URI and associated authentication key have to be verified before succesfully predicting using the deployed model
![Consume Endpoint](https://github.com/tmmsagheer/nd00333_AZMLND_C2/blob/master/starter_files/Images/endpoint.png)
8. Till now, we used a mix of Azure ML Studio and Azure Python SDK to create an AutoML experiment, deploy it and consume it. Now we will use Azure Python SDK exclusively to do the same.
![Pipeline Automation](https://github.com/tmmsagheer/nd00333_AZMLND_C2/blob/master/starter_files/Images/pipeline_2_1.png)
The above screenshot shows the automl experiment created from aml-pipelines-with-automated-machine-learning-step.ipynb notebook has completed
![Pipeline Automation](https://github.com/tmmsagheer/nd00333_AZMLND_C2/blob/master/starter_files/Images/pipeline_2_2.png)
The above screenshot shows the running status of the best model deployed as REST endpoint
![Pipeline Automation](https://github.com/tmmsagheer/nd00333_AZMLND_C2/blob/master/starter_files/Images/pipeline_2_3.png)
The above screenshot shows the Pipeline Endpoints exclusively
![Pipeline Automation](https://github.com/tmmsagheer/nd00333_AZMLND_C2/blob/master/starter_files/Images/pipeline_2_4_zoomedIn1.png)
The above screenshot shows the REST endpoint URI and the deployment status as Active
![Pipeline Automation](https://github.com/tmmsagheer/nd00333_AZMLND_C2/blob/master/starter_files/Images/pipeline_2_5.png)
The above screenshot shows the link to the endpoint in aml-pipelines-with-automated-machine-learning-step.ipynb notebook for reference
![Pipeline Automation](https://github.com/tmmsagheer/nd00333_AZMLND_C2/blob/master/starter_files/Images/pipeline_2_6.png)
The above screenshot shows the run details of Pipeline Endpoint run in aml-pipelines-with-automated-machine-learning-step.ipynb notebook for reference
![Pipeline Automation](https://github.com/tmmsagheer/nd00333_AZMLND_C2/blob/master/starter_files/Images/pipeline_2_7.png)
The above screenshot shows the same Run ID in Azure ML Studio for reference







## Screen Recording
Please find the screencast here: https://youtu.be/SkluBFWubZ8

## Standout Suggestions
*TODO (Optional):* This is where you can provide information about any standout suggestions that you have attempted.
