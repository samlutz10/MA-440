# MA-440

### Abstract

Research into the pathology of narcissism has led some to suggest that there exists two distinct but at times overlapping components to this family of behavioral characteristics. Authors Krizan and Herlache in “The Narcissism Spectrum Model (NSM): A Synthetic View” support this theory through a model of narcissism as a set of traits either leaning towards grandiosity (approach oriented) or vulnerability (response oriented) with a shared core of self-entitlement. Through statistical and cluster analysis on three datasets comprised of survey responses corresponding to the Narcissistic Personality Inventory (NPI), Hypersensitivity Narcissism Scale (HNS) , and the Dark Triad scales, we found supporting evidence for the existence of these groups and applied four machine learning algorithms (MLAs) to the task of identifying individuals as potentially “grandiose” or “vulnerable” narcissists according to the NSM. We found relatively high recalls for these classes but variable precisions indicating that the NSM might be well suited for broadly delineating groups that likely contain true narcissists as well as many false positives, especially for grandiosity.

### NPI Dataset

The Narcissistic Personality Inventory was tailored to show the more grandiose side of individuals, rather than vulnerability. Due to these types of questions, the clustering had to be closely analyzed in order to determine the vulnerability of individuals. In addition, 5 clusters were selected since the NPI data is binary. This means there were only two options for each question, which made analyzing the data much harder. The median in this case was hard to use, and the average for each question in lower cluster numbers would not give enough information about the cluster. Due to this high instability, the average answer for each question of each cluster was compared to the average answer for all clusters in each question. This proved to give a better overall understanding of how each cluster performed in each question.


