# Operationalizing Azure Machine Learning

## Project Overview
In this project, we use Azure and Azure ML studio to create cloud-based ML pipelines, which are easily automated and updatable. We create train models using AutoML, then choose and deploy the best model. The model endpoints are then consumed via REST API calls.


## Architectural Diagram
![alt text](https://github.com/jackharrison27/Azure_Machine_Learning_Operations/blob/master/screenshots/architectural_diagram.png?raw=true)


## Required Screenshots

### AutoML run
For this project, an AutoML run was completed on bank marketing dataset. The best model, a Voting Ensemble, was selected to be deployed. 
- "Registed Datasets" in ML studio
![alt text](https://github.com/jackharrison27/Azure_Machine_Learning_Operations/blob/master/screenshots/dataset.png?raw=true)

- The experiment is complete
![alt text](https://github.com/jackharrison27/Azure_Machine_Learning_Operations/blob/master/screenshots/complete_experiment.png?raw=true)

- Best model
![alt text](https://github.com/jackharrison27/Azure_Machine_Learning_Operations/blob/master/screenshots/best_model.png?raw=true)


### Enable Logging
After deployment, we turned on the "Application Insights" within the Azure Container Instance. This was done through the logs.py script since "Application Insights" is disabled by defult.   
- "Application Insights" is enabled
![alt text](https://github.com/jackharrison27/Azure_Machine_Learning_Operations/blob/master/screenshots/application_endpoint_true.png?raw=true)

- Log.py script is running
![alt text](https://github.com/jackharrison27/Azure_Machine_Learning_Operations/blob/master/screenshots/logs.png?raw=true)

### Swagger Doccumentation
We used Swagger to view the contents of the model and see what API methods are available. This allows users to view how to consume the model enpoint with HTTP request methods. In this case, we deployed the Swagger page on a localhost port. 
- Swagger runs on local host showing API methods
![alt text](https://github.com/jackharrison27/Azure_Machine_Learning_Operations/blob/master/screenshots/swagger.png?raw=true)

### Consume Model Endpoints
The model was then tested using sample JSON requests. In this case, endpoints.py was used to test the outputs of our model and the success of our API methods. 
- endpoint.py script runs
![alt text](https://github.com/jackharrison27/Azure_Machine_Learning_Operations/blob/master/screenshots/endpoint.png?raw=true)

### Pipeline 
For this part of the project, we created a pipeline through a jupyter notebook. After using a config.json file to authenticate the notebook automatically, we fed the data to another AutoML run with specific parameters as set by the notebook. The best model was then selected and deploys it. We confirmed the endpoint was created by checking the pipeline overview and that the endpoint has a status of "Active." Finally we queried the pipeline endpoint using Postman to confirm its successful deployment. 
- Pipeline has been created
![alt text](https://github.com/jackharrison27/Azure_Machine_Learning_Operations/blob/master/screenshots/pipeline.png?raw=true)

- Pipeline endpoints
![alt text](https://github.com/jackharrison27/Azure_Machine_Learning_Operations/blob/master/screenshots/pipeline_endpoint.png?raw=true)

- Bank dataset with the AutoML module
![alt text](https://github.com/jackharrison27/Azure_Machine_Learning_Operations/blob/master/screenshots/graph.png?raw=true)

- "Published Pipeline Overview," showing REST endpoint is active
![alt text](https://github.com/jackharrison27/Azure_Machine_Learning_Operations/blob/master/screenshots/active_rest_endpoint.png?raw=true)

- Jupyter Notebook, using RunDetails Widget
![alt text](https://github.com/jackharrison27/Azure_Machine_Learning_Operations/blob/master/screenshots/run_details_widget.png?raw=true)

- ML Studio showing run
![alt text](https://github.com/jackharrison27/Azure_Machine_Learning_Operations/blob/master/screenshots/endpoints.png?raw=true)

- Using Postman to query the endpoint
![alt text](https://github.com/jackharrison27/Azure_Machine_Learning_Operations/blob/master/screenshots/postman.png?raw=true)


## Future Improvements
- Use deep learning features when building models
- Use feature engineering to improve training data
- Use more data!


## Screencast 
Link to screencast of the project: https://vimeo.com/666540506
</br>
Screencast includes a demonstration of:
-  AutoML model creation
-  Deploy best model
-  Consume best model
-  Pipleine creation
-  Query with Postman

