# Udacity AzureML nanodegree - Operationalizing Machine Learning

In this exercise I'm going to use a pipeline with an automl modelsearch as a step. Once the model has been trained I will test it, deploy the endpoint and test the endpoint with a Json request.

## Architectural Diagram
![alt text](img/architectural_diagram.png?raw=true "Dataset")

## Key Steps
The steps to complete this exercise are:

  * Define workspace and experiment
  * Create or attahce computetarget
  * Load dataset from datastore
  * create automl step
  * Run pipeline
  * Fetch best model
  * Deploy model endpoint
  * Enable logging using logs.py
  * Start Swagger with swagger json from endpoint
  * Test endpoint with endpoint.py script and json request.


### **UCI Banking dataset is uploaded to datastore and registered.**
---
![alt text](img/Dataset.png?raw=true "Dataset")


### **Pipeline/training is running and we can follow the progrees in the details widget.**
---
![alt text](img/run_details_widget.png?raw=true "Run Details Widget")


### **Overview of pipeline with details.**
---
![alt text](img/pipeline_overview.png?raw=true "Pipeline")
![alt text](img/pipeline.png?raw=true "Pipeline")

### **AutoML found that the best model for this problem is a VotingEnsemble model composed of XGBoost models**
---
![alt text](img/model_completed.png?raw=true "Model")


### **Published pipeline.**
---
![alt text](img/active_pipeline.png?raw=true "Published pipeline")


### **Pipeline endpoint.**
---
![alt text](img/Pipeline_endpoint.png?raw=true "Pipeline endpoint")


### **Model endpoint with REST endpoint url, Swagger URI and application insights enabled.**
---
![alt text](img/model_endpoint.png?raw=true "Model endpoint")

### **Service Principal is started as I used my own Azure platform.**
---
![alt text](img/ServicePrincipal.png?raw=true "Service principal")


### **Workspace role is defined.**
---
![alt text](img/workspace_role.png?raw=true "Workspace role")


### **Swagger json is downloaded to swagger folder and Swagger is run.**
---
![alt text](img/swagger.png?raw=true "swagger")


### **Logging is enabled by running logs.py**
---
![alt text](img/logs_py.png?raw=true "Logs")


### **We test the model endpoint by sending it a json request and receive a prediction.**
---
![alt text](img/endpoint.png?raw=true "Endpoint tested")


## Screen Recording
*Screencast: https://youtu.be/MgPzGhnRYlA*

## Future improvements
There's still plenty of room for improvements:
  * We can do feature engineering, eg. make categorial values one-hot.
  * We can sample the target categories if they are not balanced.
  * We can fine tune the hyperparameters of the best model. Eg. using Hyperdrive.
