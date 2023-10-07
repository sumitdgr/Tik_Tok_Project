**TikTokClaimDetective: Claim or Opinion using ML**

The aim of the project is to use machine learning to extract claims or propositions within TikTok videos and comments and classify each data point as a claim or opinion. To approach this task i will be using the PACE frame-work that is an accronym for a 4 stage approach Plan, Analyze, Construct and Execute.

**Plan :**

1- Goal: To determine whether a video contains a claim or whether it offers an opinion.

2- Strategies utilized :

    Data Source : Gathered with in from the organization (first party) and provided as a csv.

    KPIs : Would depend on the insights covered via statistical inferences and machine learning algorithms and their performnace.

    Tools : Python, statsmodel, scipy, scikit-learn, Tableau and various others on need basis.

    Deliverables for Plan stage : Dataset scrubbed for EDA, visualizations, statistical model, regression analysis, and/or machine learning.

3 - Deliverables :

  Findings:

    After looking at the dataset, the two variables that are most likely to help build a predictive model are claim_status and opinion_status.     We can create a classification model to differentiate the two variables, as instructed from the employer.

    The mean is larger than the median, so the data is right-skewed. Therefore, it is recommended to consider applying a variable         
    transformation, such as taking logarithms, prior to modeling.

  Python file : Stage 1 Deliverable : Notebook

**Analyze :**

1- In this stage we will be covering the following processes:

      ETL (Extract, Transform, Load) as/if required.

      EDA (Exploratory Data Analysis) to uncover as much insights as possible.

      This stage also includes working with the stakeholders to create a subset of the insights discovered in the previous step. This subset         will    only include those insights that are to be pursued further.

2- Findings and Deliverables :

      Executive Summary : Stage 2 Deliverabe: Summary File

      Python File : Stage 2 Deliverable : Notebook

**Construct :**

1- This stage includes the following processes :

      Deciding what insights to pursue.

      Statistical Analysis

      Regression Analysis

      Utilizing Machine Learning Algorithm.

2- Starting with Statistical Analysis our next step is to find out if there is any statistical difference betweem the mean of video views count of verified and un-verified accounds. We do this by finding the p-value and if this less than our threshold of 5% we will reject the null hypothesis.

      Eexecutive Summary : Stage 3 Deliverables : Statistics Summary File

      Python File : Stage 3 Deliverables : Stats-Notebook

3- Earlier, we observed that if a user is verified, they are much more likely to post opinions. Since the end goal is to classify claims and opinions, it’s important to build a model that shows how to predict the behavior of the account type (verified) that tend to post more opinions. So, in this part of the project, we built a logistic regression model that predicts verified_status. The following files include the summary and notebook of the process.

      Executive Summary : Stage 3 Deliverables : Regression Analysis Summary
  
      Python File : Stage 3 Deliverables : Regression-Notebook

4- Now the final part comes in where we prepare the product. The following files contain the summary of the process and the model itself:

      Executive Summary : Stage 3 Deliverables : Final Product Summary File

      Python File : Stage 3 Deliverables : Product-Notebook

**Execute :**

1- This part of the framework is where we present the product to the stakeholders.

2- Our best model gave an accuracy of over 99%.
