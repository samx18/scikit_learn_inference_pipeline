# SageMaker Inference Pipeline

In the following notebook, we will demonstrate how you can build your ML Pipeline leveraging the Sagemaker Scikit-learn container and SageMaker Linear Learner algorithm & after the model is trained, deploy the Pipeline (Data preprocessing and Lineara Learner) as an Inference Pipeline behind a single Endpoint for real time inference and for batch inferences using Amazon SageMaker Batch Transform.

## Dataset
The dataset is available from UCI Machine Learning; the aim for this task is to determine age of an Abalone (a kind of shellfish) from its physical measurements. We'll use Sagemaker's Scikit-learn container to featurize the dataset so that it can be used for training with Linear Learner.


**Numeric Features:**
* length:  Longest shell measurement
* diameter: Diameter perpendicular to length
* height:  Height with meat in shell
* whole_weight: Weight of whole abalone
* shucked_weight: Weight of meat
* viscera_weight: Gut weight (after bleeding)
* shell_weight: Weight after being dried

**Categorical Features:**
* sex: categories encoded as strings {'M', 'F', 'I'} where 'I' is Infant

## Inference

rings +1.5 gives the age in years


