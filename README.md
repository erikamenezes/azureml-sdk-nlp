# Azure Machine Learning SDK - NLP

In this tutorial we will go over the data science process for a typical Natural Language Processing (NLP) project using the Azure Machine Learning SDK. This will cover the end-to-end process of data prep, model building and deployment, and consumption of the deployed model as web service. You can use these examples to as a starting point for your own projects.

## What is Azure Machine Learning?
Azure Machine Learning service is a cloud service that you use to train, deploy, automate, and manage machine learning models. It supports several deep learning frameworks, and other  libraries that are commonly used for machine leanring projects. To learn more, see the [official documentation](https://docs.microsoft.com/en-us/azure/machine-learning/service/overview-what-is-azure-ml?WT.mc_id=aisummit-github-amynic).

## Setup
You have mutltiple options for development environments to use with Azure Machine Learning. Choose the one you're most comfortable with from [here](https://docs.microsoft.com/en-us/azure/machine-learning/service/how-to-configure-environment?WT.mc_id=aisummit-github-amynic). 

For these samples specifically I have tested:
* [Data Science Virtual Machine](https://docs.microsoft.com/en-us/azure/machine-learning/service/how-to-configure-environment#azure-notebooks-and-data-science-virtual-machine?WT.mc_id=aisummit-github-amynic) in Azure 
* [Jupyter setup on your own machine](https://docs.microsoft.com/en-us/azure/machine-learning/service/how-to-configure-environment#azure-notebooks-and-data-science-virtual-machine?WT.mc_id=aisummit-github-amynic)

## What do the notebooks cover?

* [text-classification-part1-training.ipynb](https://github.com/erikamenezes/azureml-sdk-nlp/blob/master/text-classification-part1-training.ipynb)
    - Workspace and experimentation setup
    - Saving your datasets in cloud storage that can be accessed by remote compute
    - Building a text classification model for the Reuters newswire dataset using Keras and Tensorflow
    - Model training locally and on a remote cluster and run monitoring
    - Hyperparameter tuning 
    - Model management, registering and versioning the model that can be reused by others.  
* [text-classification-part2-deployment.ipynb](https://github.com/erikamenezes/azureml-sdk-nlp/blob/master/text-classification-part2-deployment.ipynb)
    - create model training and scoring scripts 
    - configure model dependencies
    - setting up a container service to host your model
    - deploying your model to the cloud container service
    - consuming and monitoring the deployed web service.

## Always remember to delete your resources 
To avoid incurring running costs make sure to delete your resources. Got to the Azure portal, search for and select your Azure machine learning service, and delete compute resources and/or the entire resource group. Also, make sure to shutdown/delete your VM when you are not using it.  

## Related recources
For more tutorials on using the Azure ML SDK, checkout the notebooks [here](https://github.com/Azure/MachineLearningNotebooks) 

Feedback on the content below is welcome 😊👍 please reach out to me on [Twitter: @erikadmenezes](https://twitter.com/erikadmenezes) or submit an [issue/pull request on github](https://github.com/erikamenezes/azureml-sdk-nlp/)
 