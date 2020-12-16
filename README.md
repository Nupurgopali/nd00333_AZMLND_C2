
# Overview of the Project
We were asked to use Azure to configure a cloud-based machine learning production model, deploy it, and consume it.Also to create, publish, and consume a pipeline.The aim of the project was to learn about Operationalizing Machine Learning model by deploying a machine learning model to an endpoint which is a URL that can be easily accessed by any end-user.

<p>In this project, the following steps were executed:
  <li>Authentication</li>
<li>Automated ML Experiment</li>
<li>Deploy the best model</li>
<li>Enable logging</li>
<li>Swagger Documentation</li>
<li>Consume model endpoints</li>
<li>Create and publish a pipeline</li>
<li>Documentation</li></p>

## Architectural Diagram

![image](https://user-images.githubusercontent.com/53776611/102314164-ffd9af80-3f97-11eb-83f6-b01844316471.png)


## Improve the Project
The project can be further improved by using different hyperparameters as it might increase the model's accuracy, using different authentication method.Tweaking parameters in the automl configurations and setting can also improve the project.These methods can be used
to improve the project.
# Screenshots

## 1.Automated ML Experiment

### Sucessfull run of AutoML model
In this step we had to create a automl model in the ML studio by adding dataset,creating compute cluster and finally successfully running the model.



![](https://github.com/Nupurgopali/nd00333_AZMLND_C2/blob/master/screenshot/completed.PNG?raw=true)


### Best model 
In this step is to figure out which is the best model(usually the model with the highest accuracy).Once the automl run is finished,it gives the best model which can be deployed.

![](https://raw.githubusercontent.com/Nupurgopali/nd00333_AZMLND_C2/master/screenshot/bestmodel.PNG)

### Run metrics of the automl model
This talk about the various factors of the best run model in automl such as its accuracy,recall,precision,etc.So that the user can decide which model they want to select.

![](https://raw.githubusercontent.com/Nupurgopali/nd00333_AZMLND_C2/master/screenshot/bestmetric2.PNG)

## 2. Enabling Logging 

### Enabling application insights in the deployed automl model
This step is used to enable the application by making the application insights of the deployed model to true.

![](https://raw.githubusercontent.com/Nupurgopali/nd00333_AZMLND_C2/master/screenshot/enable_application_insights.PNG)

## 3. Swagger Documentation
### Result of running the command: python Logs.py
To interact with the swagger UI,we first have to run logs.py file that creates a service via which we can interact with the website.For this we have to link our deployed model
to the service this is done by providing the same deployed model name as service name.
![image](https://user-images.githubusercontent.com/53776611/102201688-74571480-3eec-11eb-98a8-f1cd5ed76a66.png)

### Swagger UI
Once the logs.py file runs successfully the swagger website can be accessed using localhost.
![image](https://user-images.githubusercontent.com/53776611/102200443-dca4f680-3eea-11eb-8b08-2d75bb3ae8a8.png)

## Request status
Interaction can be done using GET and POST HTTPS methods.
![image](https://user-images.githubusercontent.com/53776611/102200977-86848300-3eeb-11eb-88e7-f89eda6e2474.png)

### Interacting using swagger ui- Swagger runnning on localhost:9000 and interacting using GET method
Here the interaction is done using the GET method of HTTPS where the information is received from the user.
![image](https://user-images.githubusercontent.com/53776611/102199483-b03caa80-3ee9-11eb-9837-651bdac04dbd.png)

### Responses of the interactiong: 
The reponse of the HTTP interaction can be visualised using POST method.
![image](https://user-images.githubusercontent.com/53776611/102200259-a0719600-3eea-11eb-95a8-3ffa4051b6d0.png)

## 4.Consume Model endpoints

### JSON Response

In order to consume the model we are suppose to provide input to the model in form of json and then check the respone that the model gives.This reponse can be further used
to analyse the performance of the model.
![image](https://user-images.githubusercontent.com/53776611/102201385-06aae880-3eec-11eb-8381-4ff7d2e0d337.png)

## 5.Create and publish a pipeline

### Creating the pipeline
The pipeline is create using automl model,configuration and setting tool.After the configuration of the model is set the pipeline is created by running it using azureml.widgets
services.
![image](https://user-images.githubusercontent.com/53776611/102201871-a9fbfd80-3eec-11eb-8320-86e4222b8145.png)

### Published Pipeline Overview
Once the pipeline is created successfully it is published using the publish option present in the menu bar.
![image](https://user-images.githubusercontent.com/53776611/102392049-92ac3580-3ffc-11eb-8691-cb79b940e466.png)


### "Registered Dataset" of the Azure ML Studio
The dataset used the train the model can be seen under the registered dataset option in the ML studio.
![image](https://user-images.githubusercontent.com/53776611/102336582-5dc9bf80-3fb7-11eb-82dd-3ea97572da3a.png)

### Pipeline Endpoint
If aa end-user wants to access the pipeline, it can be done using a pipeline endpoint.Pipeline endpoint is created once it has been published successfully.
![Capture](https://user-images.githubusercontent.com/53776611/102343449-93bf7180-3fc0-11eb-873d-f45894834a5f.PNG)


### Scheduled Run 
In this the user get the overview of different model and dataset that are ruuning with their status.
![image](https://user-images.githubusercontent.com/53776611/102343501-a639ab00-3fc0-11eb-9d3e-13066d1cfab1.png)



## URL for the video
#### LINK :https://youtu.be/0uVqUzB2A1Y
