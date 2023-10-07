Plan :
Goal: To determine whether a video contains a claim or whether it offers an opinion.
Strategies utilized :
Data Source : Gathered with in from the organization (first party) and provided as a csv.
KPIs : Would depend on the insights covered via statistical inferences and machine learning algorithms and their performnace.
Tools : Python, statsmodel, scipy, scikit-learn, Tableau and various others on need basis.
Deliverables for Plan stage : Dataset scrubbed for EDA, visualizations, statistical model, regression analysis, and/or machine learning.
Deliverables :
Findings:
After looking at the dataset, the two variables that are most likely to help build a predictive model are claim_status and opinion_status. We can create a classification model to differentiate the two variables, as instructed from the employer.
The mean is larger than the median, so the data is right-skewed. Therefore, it is recommended to consider applying a variable transformation, such as taking logarithms, prior to modeling.
Python file : Stage 1 Deliverable : Notebook
Analyze :
In this stage we will be covering the following processes:
ETL (Extract, Transform, Load) as/if required.
EDA (Exploratory Data Analysis) to uncover as much insights as possible.
This stage also includes working with the stakeholders to create a subset of the insights discovered in the previous step. This subset will only include those insights that are to be pursued further.
Findings and Deliverables :
Executive Summary : Stage 2 Deliverabe: Summary File
Python File : Stage 2 Deliverable : Notebook
Construct :
This stage includes the following processes :
Deciding what insights to pursue.
Statistical Analysis
Regression Analysis
Utilizing Machine Learning Algorithm.
Starting with Statistical Analysis our next step is to find out if there is any statistical difference betweem the mean of video views count of verified and un-verified accounds. We do this by finding the p-value and if this less than our threshold of 5% we will reject the null hypothesis.
Eexecutive Summary : Stage 3 Deliverables : Statistics Summary File
Python File : Stage 3 Deliverables : Stats-Notebook
Earlier, we observed that if a user is verified, they are much more likely to post opinions. Since the end goal is to classify claims and opinions, it’s important to build a model that shows how to predict the behavior of the account type (verified) that tend to post more opinions. So, in this part of the project, we built a logistic regression model that predicts verified_status. The following files include the summary and notebook of the process.
Executive Summary : Stage 3 Deliverables : Regression Analysis Summary
Python File : Stage 3 Deliverables : Regression-Notebook
Now the final part comes in where we prepare the product. The following files contain the summary of the process and the model itself:
Executive Summary : Stage 3 Deliverables : Final Product Summary File
Python File : Stage 3 Deliverables : Product-Notebook
Execute :
This part of the framework is where we present the product to the stakeholders.
Our best model gave an accuracy of over 99%.
# Tik_Tok_Project

# 1 - Python
Welcome to the TikTok Project!

You have just started as a data professional at TikTok.

The team is still in the early stages of the project. You have received notice that TikTok's leadership team has approved the project proposal. To gain clear
insights to prepare for a claims classification model, TikTok's provided data must be examined to begin the process of exploratory data analysis (EDA).

# 2 - Exploratory data analysis

Your TikTok data team is still in the early stages of their latest project. So far, you’ve completed a project proposal and used Python to inspect and organize
the TikTok dataset.

Orion Rainier, a Data Scientist at TikTok, is pleased with the work you have already completed and is requesting your assistance with some Exploratory Data Analysis
(EDA) and data visualization. The management team asked to see a Python notebook showing data structuring and cleaning, as well as any matplotlib/seaborn
visualizations plotted to help us understand the data. At the very least, include a graph comparing claim counts to opinion counts, as well as boxplots of the most
important variables (like “video duration,” “video like count,” “video comment count,” and “video view count”) to check for outliers. Also, include a breakdown of
“author ban status” counts.

Additionally, the management team has recently asked all EDA to include Tableau visualizations. Tableau visualizations are particularly helpful in status reports
to the client and board members. For this data, create a Tableau dashboard showing a simple claims versus opinions count, as well as stacked bar charts of claims
versus opinions for variables like video view counts, video like counts, video share counts, and video download counts. Make sure it is easy to understand to someone
who isn’t data savvy, and remember that the assistant director is a person with visual impairments.

You also notice a follow-up email from the Data Science Lead, Willow Jaffey. Willow suggests including an executive summary of your analysis to share with teammates.

# 3 - Statistic

You are a data professional at TikTok. The current project is reaching its midpoint; a project proposal, Python coding work, and exploratory data analysis have
all been completed.

The team has reviewed the results of the exploratory data analysis and the previous executive summary the team prepared. You received an email from Orion Rainier,
Data Scientist at TikTok, with your next assignment: determine and conduct the necessary hypothesis tests and statistical analysis for the TikTok classification
project.

# 4 - Regression Analysis

You are a data professional at TikTok. The data team is working towards building a machine learning model that can be used to determine whether a video contains
a claim or whether it offers an opinion. With a successful prediction model, TikTok can reduce the backlog of user reports and prioritize them more efficiently.

The team is getting closer to completing the project, having completed an initial plan of action, initial Python coding work, EDA, and hypothesis testing.

The TikTok team has reviewed the results of the hypothesis testing. TikTok’s Operations Lead, Maika Abadi, is interested in how different variables are
associated with whether a user is verified. Earlier, the data team observed that if a user is verified, they are much more likely to post opinions. Now, the
data team has decided to explore how to predict verified status to help them understand how video characteristics relate to verified users. Therefore, you
have been asked to conduct a logistic regression using verified status as the outcome variable. The results may be used to inform the final model related to
predicting whether a video is a claim vs an opinion.

# 5 - Machine Learning

Recall that you are a data professional at TikTok. Your supervisor was impressed with the work you have done and has requested that you build a machine
learning model that can be used to determine whether a video contains a claim or whether it offers an opinion. With a successful prediction model, TikTok
can reduce the backlog of user reports and prioritize them more efficiently.
