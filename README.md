# Sparkify Capstone Project

## 1. Installation
I use python 3.5 to create this project and the main libraries I used are:
- ibmos2spark==1.0.1
- matplotlib==2.1.0
- numpy==1.13.3
- pandas==0.21.0
- pyspark==2.3.0
- seaborn==0.8

Please check requirement.txt for the detailed packages information.

## 2. Project Motivation
The Udacity Capstone project is to predict churn rate.  customer-facing business often  face the challenge of losing customers and need to take actions to keep customers. Predicting churn rates is a common problem that data scientists regularly encounter in lots of customer-facing business.
Secondly,the ability to efficiently manipulate large datasets with Spark is one of the highest-demand skills in the big data domain. This project improves my spark skills essentially with:
 - Learn how to create a spark cluster on the cloud platform like IBM, AWS.
 - How to Manipulate large and realistic datasets with Spark to engineer relevant features for predicting churn.
 - How to Use Spark MLlib to build machine learning models on big data, far beyond what could be done with non-distributed technologies like scikit-learn.

## 3. File Descriptions

- Spark capstone project\
   - README.md
   - cluster-overview.png
   - Sparkify.ipynb
   - requirements.txt

## 4.Instructions:

     1. Create a spark cluster that consists of one driver and 2 executors on the IBM cloud. Its architecture is shown as follows:
![Spark cluster](cluster-overview.png 'cluster-overview')
     2. Download the  medium sized dataset that includes sparkify user behavior logs.

     3. Create  Sparkify.ipynb to predict churn rate. It following the CRISP-DM process.
## 5. Result:
Finally, three classifiers get the following scores:
- GBTClassifier
 - Training: accuracy: 95.39%, Precision: 97.02%, Recall: 95.39%, F1 Score: 95.22%
 - Test:	 accuracy: 84.93%, Precision: 87.40%, Recall: 84.93%, F1 Score: 84.28%
- LogisticRegression:
 - Training: accuracy: 80.22%, Precision: 79.28%, Recall: 81.03%, F1 Score: 74.16%
 - Test:	 accuracy: 79.45%, Precision: 62.67%, Recall: 76.71%, F1 Score: 74.39%
- RandomForestClassifier
 - Training: accuracy: 90.24%, Precision: 89.84%, Recall: 90.79%, F1 Score: 90.40%
 - Test:	 accuracy: 90.41%, Precision: 90.38%, Recall: 90.41%, F1 Score: 89.65%

The highest f1 average score model is 89.65%. The best performing model for the first iteration was RandomForestClassifier. Its variance and bias are low while training scores compare with test scores.  So it means RandomForestClassifier generalization on the test dataset performs better than other classifiers. While this is a good first iteration step, there is still a lot of work to do before the model is released into production.

## 6. Web link:
   - GitHub: https://github.com/bin-wang-sh/sparkify_capstone_project
   - Blog: https://blog.csdn.net/nettravel_sh/article/details/86602116

## 7 Acknowledgement

- Thank you to the @udacity staff for giving me the opportunity to uplevel my Spark skills.
- Thank Jacob Hansen for his idea about how to find useful page action.

## 8. Licensing, Author, Acknowledgements
This work is licensed under a [Creative Commons  Attribution-NonCommercial-NoDerivatives 4.0 International License](http://creativecommons.org/licenses/by-nc-nd/4.0/). Please refer to [Udacity Terms of Service](https://www.udacity.com/legal) for further information.
