# Credit Risk Analysis
## Introduction
#### Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, 6 different Maching Learning models will be used to predict credit risk. Based on these the performance of these models will be evaluated to make a recommendation on whether they should be used to predict credit risk.
## Results
### The 6 models will include 4 Algorithms: Naive Random oversampling, SMOTE oversampling, Cluster Centroids undersampling and SMOTEENN over & under sampling along with 2 ensemble classifiers:  Balanced Random Forest and Easy Ensemble 
####  The results for each are pictured below, with an analysis based on the confusion matrices, accuracy score, and imblanced classification report.  
####  Although it is not always the most appropriate or meaningful metric, the accuracy score can be included in the many ways to determine if a model is valid.  The other 3 are precision, sensitivity, and the balance of both in the F1 score.  A test high in sensitivity may do a good job finding the target but will risk a number of false positives.  On the otherhand, for tests high in precision, there is high confidence that the predicted positives are indeed positive, but at the risk of not predicting all true positives.  Finally the higher the F1 score the better balance between sensitivity and precision which would indicate a better model.  
#### General Confusion Matrix
![Confusion Matrix](https://user-images.githubusercontent.com/115171651/226054230-40e48bce-8949-437c-b7f9-694d10199daa.png)

#### Naive Random Oversampling
![Naive_ROS](https://user-images.githubusercontent.com/115171651/226050659-d62844f9-9ecd-40c2-80d7-fa6dc0ba022c.png)
#### SMOTE Oversampling
![SMOTE_OS](https://user-images.githubusercontent.com/115171651/226050672-d927dbf5-187f-4990-bcc5-a63ae42270f2.png)
#### Cluster Centroid Undersampling
![Undersampling](https://user-images.githubusercontent.com/115171651/226050716-0f4f1297-8ee7-4788-bcac-56a3e7944891.png)
#### SMOTEENN Over and Undersampling
![Combo_Over_Under_Sampling](https://user-images.githubusercontent.com/115171651/226050766-54f39808-4853-4a4e-9b11-18d881c6581b.png)
#### Balanced Random Forest
![Balanced_Random_Forest](https://user-images.githubusercontent.com/115171651/226050805-d493547b-c43e-4ec0-97d5-d44cd7d120ba.png)
#### Easy Ensemble
![Easy_ensemble_adaboost](https://user-images.githubusercontent.com/115171651/226050829-e57a7de9-1bbd-474f-8c23-30fd9e775544.png)
## Summary & Recommendation
#### 5 of the 6 models had very similar accuracy scores around 0.65 but there is a very distinct differences between the 4 algorithms and the 2 ensemble classifiers.  The 2 oversampling methods were closer in the precision and recall scores with the undersampling being different.  The combination of the over and undersampling was not sigficantly different than the oversampling models.  The 4 sampling methods were not very good at precision when it came to high-risk credit. 

#### The two ensemble methods were significantly higher in the precision of the high and low risk credit,  Overall their numbers were higher in all the categories except for recall.  

#### I have no recommendation in that I am still unsure which model type is the best.  Given that there is such a hugh disparity in the false negatives, which doesn't seem to be explained in this data.  One reason there is concern is it would seem that the actual positive number should be similar and the difference would be whether or not the prediction was correct.  Instead the differeneces between the first 4 and last 2 are made up in the true negative box.  That doesn't seem to make any sense.  


