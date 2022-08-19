# Use sample datasets<a name="canvas-sample-datasets"></a>

SageMaker Canvas provides sample datasets addressing unique use cases so you can start building, training, and validating models quickly without writing any code\. The use cases associated with these datasets highlight the capabilities of SageMaker Canvas, and you can leverage these datasets to get started with building models\. You can find the sample datasets in the **Datasets** page of your SageMaker Canvas application\.

## Sample datasets<a name="canvas-sample-datasets-list"></a>

The following datasets are the samples that SageMaker Canvas provides by default\. These datasets cover use cases such as predicting house prices, loan defaults, and readmission for diabetic patients; forecasting sales; predicting machine failures to streamline predictive maintenance in manufacturing units; and generating supply chain predictions for transportation and logistics\. The datasets are stored in the `sample_dataset` folder in the default Amazon S3 bucket that SageMaker creates for your account in a Region\.
+ **canvas\-sample\-diabetic\-readmission\.csv:** This dataset contains historical data including over fifteen features with patient and hospital outcomes\. You can use this dataset to predict whether high\-risk diabetic patients are likely to get readmitted to the hospital within 30 days of discharge, after 30 days, or not at all\. Use the **redadmitted** column as the target column, and use the 3\+ category prediction model type with this dataset\. To learn more about how to build a model with this dataset, see the [SageMaker Canvas workshop page](https://catalog.us-east-1.prod.workshops.aws/workshops/80ba0ea5-7cf9-4b8c-9d3f-1cd988b6c071/en-US/5-hcls)\. This dataset was obtained from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/diabetes+130-us+hospitals+for+years+1999-2008)\. 
+ **canvas\-sample\-housing\.csv:** This dataset contains data on the characteristics tied to a given housing price\. You can use this dataset to predict housing prices\. Use the **median\_house\_value** column as the target column, and use the Numeric prediction model type with this dataset\. To learn more about building a model with this dataset, see the [SageMaker Canvas workshop page](https://catalog.us-east-1.prod.workshops.aws/workshops/80ba0ea5-7cf9-4b8c-9d3f-1cd988b6c071/en-US/2-real-estate)\. This is the California housing dataset obtained from the [StatLib repository](https://www.dcc.fc.up.pt/~ltorgo/Regression/cal_housing.html)\.
+ **canvas\-sample\-loans\.csv:** This dataset contains complete loan data for all loans issued from 2007–2011, including the current loan status and latest payment information\. You can use this dataset to predict whether a customer will repay a loan\. Use the **loan\_status** column as the target column, and use the 3\+ category prediction model type with this dataset\. To learn more about how to build a model with this dataset, see the [SageMaker Canvas workshop page](https://catalog.us-east-1.prod.workshops.aws/workshops/80ba0ea5-7cf9-4b8c-9d3f-1cd988b6c071/en-US/4-finserv)\. This data uses the LendingClub data obtained from [Kaggle](https://www.kaggle.com/datasets/wordsforthewise/lending-club)\.
+ **canvas\-sample\-maintenance\.csv:** This dataset contains data on the characteristics tied to a given maintenance failure type\. You can use this dataset to predict which failure will occur in the future\. Use the **Failure Type** column as the target column, and use the 3\+ category prediction model type with this dataset\. To learn more about how to build a model with this dataset, see the [SageMaker Canvas workshop page](https://catalog.us-east-1.prod.workshops.aws/workshops/80ba0ea5-7cf9-4b8c-9d3f-1cd988b6c071/en-US/6-manufacturing/)\. This dataset was obtained from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/AI4I+2020+Predictive+Maintenance+Dataset)\.
+ **canvas\-sample\-shipping\-logs\.csv:** This dataset contains complete shipping data for all products delivered, including estimated time shipping priority, carrier, and origin\. You can use this dataset to predict the estimated time of arrival of the shipment in number of days\. Use the **ActualShippingDays** column as the target column, and use the Numeric prediction model type with this dataset\. To learn more about how to build a model with this data, see the [SageMaker Canvas workshop page](https://catalog.us-east-1.prod.workshops.aws/workshops/80ba0ea5-7cf9-4b8c-9d3f-1cd988b6c071/en-US/7-supply-chain/)\. This is a synthetic dataset created by Amazon\.
+ **canvas\-sample\-sales\-forecasting\.csv:** This dataset contains historical time series sales data for retail stores\. You can use this dataset to forecast sales for a particular retail store\. Use the **sales** column as the target column, and use the Time series forecasting model type with this dataset\. To learn more about how to build a model with this dataset, see the [SageMaker Canvas workshop page](https://catalog.us-east-1.prod.workshops.aws/workshops/80ba0ea5-7cf9-4b8c-9d3f-1cd988b6c071/en-US/3-retail/)\. This is a synthetic dataset created by Amazon\.

## Re\-import a deleted sample dataset<a name="canvas-sample-datasets-reimport"></a>

If you no longer wish to use the sample datasets, you can delete them from the **Datasets** page of your SageMaker Canvas application\. However, these datasets are still stored in the default SageMaker\-created Amazon S3 bucket for your account, so you can always access them later\.

The default Amazon S3 bucket name where the datasets are stored follows the pattern `sagemaker-{region}-{account ID}`\. You can find the sample datasets in the directory path `Canvas/sample_dataset`\.

If you delete a sample dataset from your SageMaker Canvas application and want to access the sample dataset again, use the following procedure\.

1. Navigate to the **Datasets** page in your SageMaker Canvas application\.

1. Choose **Import data**\.

1. From the list of S3 buckets, select the default SageMaker S3 bucket for your account, which follows the naming pattern `sagemaker-{region}-{account ID}`\.

1. Select the **Canvas** folder\.

1. Select the **sample\_dataset** folder, which contains all of the sample datasets for SageMaker Canvas\.

1. Select the dataset you want to import, and then choose **Import data**\.