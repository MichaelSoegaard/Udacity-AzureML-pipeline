# Udacity AzureML nanodegree - Operationalizing Machine Learning

In this exercise I'm going to use a pipeline with an automl modelsearch as a step. Once the model has been trained I will test it, deploy the endpoint and test the endpoint with a Json request.

## Architectural Diagram
*TODO*: Provide an architectual diagram of the project and give an introduction of each step. An architectural diagram is an image that helps visualize the flow of operations from start to finish. In this case, it has to be related to the completed project, with its various stages that are critical to the overall flow. For example, one stage for managing models could be "using Automated ML to determine the best model". 

## Key Steps
The steps to complete this exercise are:

  * Define workspace and experiment
  * Create or attahce computetarget
  * Load dataset from datastore
  * create automl step
  * Run pipeline
  * Fetch best model
  * Deploy model endpoint
  * Start Swagger with swagger json from endpoint
  * Test endpoint with endpoint.py script and json request.

## Screen Recording
*Screencast: https://youtu.be/MgPzGhnRYlA*

## Future improvements
There's still plenty of room for improvements:
  * We can do feature engineering, eg. make categorial values one-hot.
  * We can sample the target categories if they are not balanced.
  * We can fine tune the hyperparameters of the best model. Eg. using Hyperdrive.
