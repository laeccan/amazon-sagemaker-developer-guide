# Amazon SageMaker Developer Guide

-----
*****Copyright &copy; 2018 Amazon Web Services, Inc. and/or its affiliates. All rights reserved.*****

-----
Amazon's trademarks and trade dress may not be used in 
     connection with any product or service that is not Amazon's, 
     in any manner that is likely to cause confusion among customers, 
     or in any manner that disparages or discredits Amazon. All other 
     trademarks not owned by Amazon are the property of their respective
     owners, who may or may not be affiliated with, connected to, or 
     sponsored by Amazon.

-----
## Contents
+ [What Is Amazon SageMaker?](whatis.md)
+ [How It Works](how-it-works.md)
   + [Machine Learning with Amazon SageMaker](how-it-works-mlconcepts.md)
   + [Training a Model with Amazon SageMaker](how-it-works-training.md)
   + [Deploying a Model on Amazon SageMaker Hosting Services](how-it-works-hosting.md)
   + [Using an Amazon SageMaker Notebook Instance to Explore and Preprocess Data](how-it-works-notebooks-instances.md)
   + [Validating Machine Learning Models](how-it-works-model-validation.md)
   + [The Amazon SageMaker Programming Model](how-it-works-prog-model.md)
+ [Getting Started](gs.md)
   + [Step 1: Setting Up](gs-set-up.md)
      + [Step 1.1: Create an AWS Account and an Administrator User](gs-account.md)
      + [Step 1.2: Create an S3 Bucket](gs-config-permissions.md)
   + [Step 2: Create an Amazon SageMaker Notebook Instance](gs-setup-working-env.md)
   + [Step 3: Train a Model with a Built-in Algorithm and Deploy It](ex1.md)
      + [Step 3.1: Create a Juypter Notebook and Initialize Variables](ex1-prepare.md)
      + [Step 3.2: Download, Explore, and Transform the Training Data](ex1-preprocess-data.md)
         + [Step 3.2.1: Download the MNIST Dataset](ex1-preprocess-data-pull-data.md)
         + [Step 3.2.2: Explore the Training Dataset](ex1-preprocess-data-inspect.md)
         + [Step 3.2.3: Transform the Training Dataset and Upload It to S3](ex1-preprocess-data-transform.md)
      + [Step 3.3: Train a Model](ex1-train-model.md)
         + [Step 3.3.1: Choose the Training Algorithm](ex1-train-model-select-algorithm.md)
         + [Step 3.3.2: Create a Training Job](ex1-train-model-create-training-job.md)
      + [Step 3.4: Deploy the Model to Amazon SageMaker Hosting Services](ex1-deploy-model.md)
      + [Step 3.5: Validate the Model](ex1-test-model.md)
   + [Step 4: Clean up](ex1-cleanup.md)
   + [Step 5: Additional Considerations: Integrating Amazon SageMaker Endpoints into Internet-facing Applications](getting-started-client-app.md)
+ [Using Built-in Algorithms with Amazon SageMaker](algos.md)
   + [Algorithms Provided by Amazon SageMaker: Common Information](common-info-all-im-models.md)
      + [Algorithms Provided by Amazon SageMaker: Common Parameters](sagemaker-algo-docker-registry-paths.md)
      + [Algorithms Provided by Amazon SageMaker: Common Data Formats](sagemaker-algo-common-data-formats.md)
         + [Common Data Formats—Training](cdf-training.md)
         + [Common Data Formats—Inference](cdf-inference.md)
      + [Algorithms Provided by Amazon SageMaker: Suggested Instance Types](cmn-info-instance-types.md)
      + [Algorithms Provided by Amazon SageMaker: Logs](common-info-all-im-models-logs.md)
   + [Linear Learner](linear-learner.md)
      + [How It Works](ll_how-it-works.md)
      + [Linear Learner Hyperparameters](ll_hyperparameters.md)
      + [Linear Learner Response Formats](LL-in-formats.md)
   + [Factorization Machines](fact-machines.md)
      + [How Factorization Machines Work](fact-machines-howitworks.md)
      + [Factorization Machines Hyperparameters](fact-machines-hyperparameters.md)
      + [Factorization Machine Response Formats](fm-in-formats.md)
   + [XGBoost Algorithm](xgboost.md)
      + [How XGBoost Works](xgboost-HowItWorks.md)
      + [XGBoost Hyperparameters](xgboost_hyperparameters.md)
   + [Image Classification Algorithm](image-classification.md)
      + [How Image Classification Works](IC-HowItWorks.md)
      + [Hyperparameters](IC-Hyperparameter.md)
   + [Amazon SageMaker Sequence2Sequence](seq-2-seq.md)
      + [How Sequence2Sequence Works](seq-2-seq-howitworks.md)
      + [Sequence2Sequence Hyperparameters](seq-2-seq-hyperparameters.md)
   + [K-Means Algorithm](k-means.md)
      + [How K-Means Clustering Works](algo-kmeans-tech-notes.md)
      + [K-Means Hyperparameters](k-means-api-config.md)
      + [k-means Response Formats](km-in-formats.md)
   + [Principal Component Analysis (PCA)](pca.md)
      + [How PCA Works](how-pca-works.md)
      + [PCA Hyperparameters](PCA-reference.md)
      + [PCA Response Formats](PCA-in-formats.md)
   + [Latent Dirichlet Allocation (LDA)](lda.md)
      + [How LDA Works](lda-how-it-works.md)
      + [LDA Hyperparameters](lda_hyperparameters.md)
   + [Neural Topic Model (NTM)](ntm.md)
      + [NTM Hyperparameters](ntm_hyperparameters.md)
      + [NTM Response Formats](ntm-in-formats.md)
   + [DeepAR Forecasting](deepar.md)
      + [DeepAR Hyperparameters](deepar_hyperparameters.md)
      + [DeepAR Request and Response Formats](deepar-in-formats.md)
   + [BlazingText](blazingtext.md)
      + [BlazingText Hyperparameters](blazingtext_hyperparameters.md)
+ [Automatically Scaling Amazon SageMaker Models](endpoint-auto-scaling.md)
   + [Configure Automatic Scaling for a Variant](endpoint-auto-scaling-add-policy.md)
   + [Editing a Scaling Policy](endpoint-auto-scaling-edit.md)
   + [Deleting a Scaling Policy](endpoint-auto-scaling-delete.md)
   + [Load Testing for Variant Automatic Scaling](endpoint-scaling-loadtest.md)
   + [Additional Considerations for Configuring Automatic Scaling](endpoint-auto-scaling-considerations.md)
+ [Using Your Own Algorithms with Amazon SageMaker](your-algorithms.md)
   + [Using Your Own Training Algorithms](your-algorithms-training-algo.md)
   + [Using Your Own Inference Code](your-algorithms-inference-code.md)
   + [Example: Using Your Own Algorithms](adv-bring-own-examples.md)
+ [Using TensorFlow with Amazon SageMaker](tf.md)
   + [Writing Custom TensorFlow Model Training and Inference Code](tf-training-inference-code-template.md)
   + [Examples: Using Amazon SageMaker with TensorFlow](tf-examples.md)
      + [TensorFlow Example 1: Using the tf.estimator](tf-example1.md)
         + [Step 1: Create a Notebook and Initialize Variables](tf-example1-prepare.md)
         + [Step 2: Train a Model on Amazon SageMaker Using TensorFlow Custom Code](tf-example1-train.md)
         + [Step 3: Deploy the Trained Model](tf-example1-deploy.md)
         + [Step 4: Invoke the Endpoint to Get Inferences](tf-example1-invoke.md)
+ [Using Apache MXNet with Amazon SageMaker](mxnet.md)
   + [Writing Custom Apache MXNet Model Training and Inference Code](mxnet-training-inference-code-template.md)
   + [Examples: Using Amazon SageMaker with Apache MXNet](sagemaker-examples.md)
      + [Apache MXNet Example 1: Using the Module API](mxnet-example1.md)
         + [Step 1: Create a Notebook and Initialize Variables](mxnet-example1-prepare.md)
         + [Step 2: Train a Model on Amazon SageMaker Using Apache MXNet Custom Code](mxnet-part1-train.md)
         + [Step 3 : Deploy the Trained Model](mxnet-example1-deploy.md)
         + [Step 4 : Invoke the Endpoint to Get Inferences](mxnet-example-invoke.md)
+ [Using Apache Spark with Amazon SageMaker](apache-spark.md)
   + [Example 1: Using Amazon SageMaker for Training and Inference with Apache Spark](apache-spark-example1.md)
      + [Using Custom Algorithms for Model Training and Hosting on Amazon SageMaker with Apache Spark](apache-spark-example1-cust-algo.md)
      + [Using the SageMakerEstimator in a Spark Pipeline](apache-spark-example1-extend-pipeline.md)
   + [Additional Examples: Using Amazon SageMaker with Apache Spark](apache-spark-additional-examples.md)
+ [Amazon SageMaker Libraries](libraries.md)
+ [Authentication and Access Control for Amazon SageMaker](authentication-and-access-control.md)
   + [Overview of Managing Access Permissions to Your Amazon SageMaker Resources](access-control-overview.md)
   + [Using Identity-based Policies (IAM Policies) for Amazon SageMaker](using-identity-based-policies.md)
   + [Amazon SageMaker API Permissions: Actions, Permissions, and Resources Reference](api-permissions-reference.md)
   + [Amazon SageMaker Roles](sagemaker-roles.md)
+ [Monitoring Amazon SageMaker](monitoring-overview.md)
   + [Monitoring Amazon SageMaker with Amazon CloudWatch](monitoring-cloudwatch.md)
   + [Logging Amazon SageMaker with Amazon CloudWatch](logging-cloudwatch.md)
   + [Logging Amazon SageMaker API Calls with AWS CloudTrail](logging-using-cloudtrail.md)
+ [Guidelines and Limits](appendix.md)
   + [Notebook Instance Security](appendix-additional-considerations.md)
   + [Save Updated Sample Notebooks in a New Location](save-notebook-updates.md)
   + [Supported Versions](supported-versions.md)
+ [API Reference](API_Reference.md)
   + [Actions](API_Operations.md)
      + [Amazon SageMaker Service](API_Operations_Amazon_SageMaker_Service.md)
         + [AddTags](API_AddTags.md)
         + [CreateEndpoint](API_CreateEndpoint.md)
         + [CreateEndpointConfig](API_CreateEndpointConfig.md)
         + [CreateModel](API_CreateModel.md)
         + [CreateNotebookInstance](API_CreateNotebookInstance.md)
         + [CreatePresignedNotebookInstanceUrl](API_CreatePresignedNotebookInstanceUrl.md)
         + [CreateTrainingJob](API_CreateTrainingJob.md)
         + [DeleteEndpoint](API_DeleteEndpoint.md)
         + [DeleteEndpointConfig](API_DeleteEndpointConfig.md)
         + [DeleteModel](API_DeleteModel.md)
         + [DeleteNotebookInstance](API_DeleteNotebookInstance.md)
         + [DeleteTags](API_DeleteTags.md)
         + [DescribeEndpoint](API_DescribeEndpoint.md)
         + [DescribeEndpointConfig](API_DescribeEndpointConfig.md)
         + [DescribeModel](API_DescribeModel.md)
         + [DescribeNotebookInstance](API_DescribeNotebookInstance.md)
         + [DescribeTrainingJob](API_DescribeTrainingJob.md)
         + [ListEndpointConfigs](API_ListEndpointConfigs.md)
         + [ListEndpoints](API_ListEndpoints.md)
         + [ListModels](API_ListModels.md)
         + [ListNotebookInstances](API_ListNotebookInstances.md)
         + [ListTags](API_ListTags.md)
         + [ListTrainingJobs](API_ListTrainingJobs.md)
         + [StartNotebookInstance](API_StartNotebookInstance.md)
         + [StopNotebookInstance](API_StopNotebookInstance.md)
         + [StopTrainingJob](API_StopTrainingJob.md)
         + [UpdateEndpoint](API_UpdateEndpoint.md)
         + [UpdateEndpointWeightsAndCapacities](API_UpdateEndpointWeightsAndCapacities.md)
         + [UpdateNotebookInstance](API_UpdateNotebookInstance.md)
      + [Amazon SageMaker Runtime](API_Operations_Amazon_SageMaker_Runtime.md)
         + [InvokeEndpoint](API_runtime_InvokeEndpoint.md)
   + [Data Types](API_Types.md)
      + [Amazon SageMaker Service](API_Types_Amazon_SageMaker_Service.md)
         + [AlgorithmSpecification](API_AlgorithmSpecification.md)
         + [Channel](API_Channel.md)
         + [ContainerDefinition](API_ContainerDefinition.md)
         + [DataSource](API_DataSource.md)
         + [DesiredWeightAndCapacity](API_DesiredWeightAndCapacity.md)
         + [EndpointConfigSummary](API_EndpointConfigSummary.md)
         + [EndpointSummary](API_EndpointSummary.md)
         + [ModelArtifacts](API_ModelArtifacts.md)
         + [ModelSummary](API_ModelSummary.md)
         + [NotebookInstanceSummary](API_NotebookInstanceSummary.md)
         + [OutputDataConfig](API_OutputDataConfig.md)
         + [ProductionVariant](API_ProductionVariant.md)
         + [ProductionVariantSummary](API_ProductionVariantSummary.md)
         + [ResourceConfig](API_ResourceConfig.md)
         + [S3DataSource](API_S3DataSource.md)
         + [StoppingCondition](API_StoppingCondition.md)
         + [Tag](API_Tag.md)
         + [TrainingJobSummary](API_TrainingJobSummary.md)
      + [Amazon SageMaker Runtime](API_Types_Amazon_SageMaker_Runtime.md)
   + [Common Errors](CommonErrors.md)
   + [Common Parameters](CommonParameters.md)
+ [Document History for Amazon SageMaker](doc-history.md)
+ [AWS Glossary](glossary.md)