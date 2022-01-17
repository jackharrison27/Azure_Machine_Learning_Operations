# Operationalizing Azure Machine Learning

## Project Overview
This project shows an example of the product of cloud-based machine learning pipelines. We deploy models, create web-based endpoints, and consume the endpoints using Azure and Azure ML.

## Architectural Diagram
![alt text](https://github.com/jackharrison27/Azure_Machine_Learning_Operations/blob/master/screenshots/architectural_diagram.png?raw=true)


## Required Screenshots

### AutoML run
- "Registed Datasets" in ML studio
![alt text](https://github.com/jackharrison27/Azure_Machine_Learning_Operations/blob/master/screenshots/dataset.png?raw=true)

- The experiment is complete
![alt text](https://github.com/jackharrison27/Azure_Machine_Learning_Operations/blob/master/screenshots/complete_experiment.png?raw=true)

- Best model
![alt text](https://github.com/jackharrison27/Azure_Machine_Learning_Operations/blob/master/screenshots/best_model.png?raw=true)


### Enable Logging
- "Application Insights" is enabled
![alt text](https://github.com/jackharrison27/Azure_Machine_Learning_Operations/blob/master/screenshots/application_endpoint_true.png?raw=true)

- Log.py script is running
![alt text](https://github.com/jackharrison27/Azure_Machine_Learning_Operations/blob/master/screenshots/logs.png?raw=true)

### Swagger Doccumentation
- Swagger runs on local host showing API methods
![alt text](https://github.com/jackharrison27/Azure_Machine_Learning_Operations/blob/master/screenshots/swagger.png?raw=true)

### Consume Model Endpoints
- endpoint.py script runs
![alt text](https://github.com/jackharrison27/Azure_Machine_Learning_Operations/blob/master/screenshots/endpoint.png?raw=true)

### Pipeline 
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

