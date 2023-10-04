# MA-440

### Abstract

Research into the pathology of narcissism has led some to suggest that there exists two distinct but at times overlapping components to this family of behavioral characteristics. Authors Krizan and Herlache in “The Narcissism Spectrum Model (NSM): A Synthetic View” support this theory through a model of narcissism as a set of traits either leaning towards grandiosity (approach oriented) or vulnerability (response oriented) with a shared core of self-entitlement. Through statistical and cluster analysis on three datasets comprised of survey responses corresponding to the Narcissistic Personality Inventory (NPI), Hypersensitivity Narcissism Scale (HNS) , and the Dark Triad scales, we found supporting evidence for the existence of these groups and applied four machine learning algorithms (MLAs) to the task of identifying individuals as potentially “grandiose” or “vulnerable” narcissists according to the NSM. We found relatively high recalls for these classes but variable precisions indicating that the NSM might be well suited for broadly delineating groups that likely contain true narcissists as well as many false positives, especially for grandiosity.

### NPI Dataset

The Narcissistic Personality Inventory was tailored to show the more grandiose side of individuals, rather than vulnerability. Due to these types of questions, the clustering had to be closely analyzed in order to determine the vulnerability of individuals. In addition, 5 clusters were selected since the NPI data is binary. This means there were only two options for each question, which made analyzing the data much harder. The median in this case was hard to use, and the average for each question in lower cluster numbers would not give enough information about the cluster. Due to this high instability, the average answer for each question of each cluster was compared to the average answer for all clusters in each question. This proved to give a better overall understanding of how each cluster performed in each question.

### Results

K-Nearest Neighbor was applied to the training and testing sets for the Dark Triad survey. By using the training dataset, a model was trained and the K parameter was fine tuned for maximum performance. The procedure for developing this model will be explained, along with the optimal parameter, the accuracy of the model, and the confusion matrix. 

To begin, the labeled training set came from the Dark Triad dataset. The model was built using this training set and then run with the testing dataset. In order to optimize the model, a for loop was run in order to determine the error rate for each of the models with an odd K value between 1 and 200. The following are the results from this model:

Optimal K Value: 89

Training Accuracy: 92.57%

Testing Accuracy: 80.30%

Although the optimal K parameter is 201 according to the graphic below, the higher the K value, the more likely for overfitting. Therefore, in order to generalize the model and reduce the effects of overfitting, a K value of 89 will be used. This K value gives an accuracy of 80.3% and was assigned by taking the square root of the number of instances in the dataset, which was 8000.

The K parameter was one of the most important in the KNN algorithm since it controls how the model predicts unlabeled data points. In order to select the best K parameter, the model was run with a set of K values between 1 and 200 and only being odd. These values had to be odd in order to prevent ties in between labels. Furthermore, the error rate was calculated for each K value and then graphed to determine the minimum.




