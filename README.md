# TITLE : Exploring Machine Learning Techniques- Sampling Methods and Model Evaluation
By Aman Verma 102103043 B.E Computer Engineering ,TIET Patiala

# 1. Methodology
![image](https://github.com/iosaman503/102103043_Sampling/assets/90442567/98071500-447b-4fc5-bcd4-130d346303b0)

# 2. Description
## Stage 1 :
In this Assignment, We were given a Credit Card Dataset comprising of 772 instances and 31 features, out of whixh on checking it was found that the data had 763 instance of Class 0 and only 9 instances of Class 1, pointing to the fact that the dataset is highly imbalanced.

Following Pie-Chart Shows the Class Imbalance :
![image](https://github.com/iosaman503/102103043_Sampling/assets/90442567/f54b7565-e7d9-4707-9954-fdb2cbda34a9)


## Stage 2:
In Order to balance the dataset, I used RandomOverSampler, it's an effective technique for dealing with imbalanced datasets. RandomOverSampler randomly duplicates instances from the minority class until it is balanced with the majority class. This method is simpler compared to SMOTE, as it doesn't involve creating synthetic samples but instead replicates existing minority class instances.

## Stage 3:
After Balancing the Dataset, we obtained equal number of instances for both the Classes(0 & 1).
Following are the briefings about the balanced Dataset :

Class Distribution of Balanced Dataset:
0    763
1    763
Name: Class, dtype: int64

Following Bar-Chart Shows the Class Distribution after Balncing the Dataset :
![image](https://github.com/iosaman503/102103043_Sampling/assets/90442567/a622bc85-0eff-4783-81b5-036a972c1046)


Now 5 different Sampling Techniques were applied on the Balanced Dataset ,which are mentioned as below :

(i) Simple Random Sampling:
Randomly selects a specified number of samples from the dataset without any specific criteria.

(ii)Stratified Sampling:
Divides the dataset into strata or groups based on a specific feature (e.g., class labels).

(iii)Cluster Sampling:
Divides the dataset into clusters or groups.
Randomly selects entire clusters and includes all samples within those clusters in the sample.

(iv)Bootstrap Sampling:
Creates multiple samples by randomly resampling with replacement from the original dataset.
Useful for estimating the distribution of a statistic or creating multiple datasets for model training.

(v)Systematic Sampling:
Selects samples at regular intervals after an initial random start.
Requires defining a sampling interval, and it's less prone to bias than simple random sampling.

## Stage 4:



