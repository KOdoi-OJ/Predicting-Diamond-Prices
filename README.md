# **Predicting Diamond Prices**
## Background & Objectives
This is the 1st project in the Predictive Analytics for Business Nanodegree from Udacity
This project is designed for three main reasons:
- To give you a feel for what you’ll be doing throughout the Nanodegree Program
- To introduce you to Udacity’s project submission and review process
- To make sure you feel comfortable with the basics before you begin. If it feels too easy, don't worry. We have some great stuff in store for you.
## Project Overview
A jewelry company wants to put in a bid to purchase a large set of diamonds, but is unsure how much it should bid. In this project, you will use the results from a predictive model to make a recommendation on how much the jewelry company should bid for the diamonds.
## Project Details
A diamond distributor has recently decided to exit the market and has put up a set of 3,000 diamonds up for auction. Seeing this as a great opportunity to expand its inventory, a jewelry company has shown interest in making a bid. To decide how much to bid, the company’s analytics team used a large database of diamond prices to build a linear regression model to predict the price of a diamond based on its attributes. You, as the business analysts, are tasked to apply that model to make a recommendation for how much the company should bid for the entire set of 3,000 diamonds.
The following diagram represents the analysis at a high level. Since the model is already built, your analysis will focus on the right side of the diagram. ![](https://video.udacity-data.com/topher/2017/February/58a4e35b_predictive-diagram/predictive-diagram.png)
 
The linear regression model provides an equation that you can use to predict diamond prices for the set of 3,000 diamonds. The equation is below:
> **Price** = -5,269 + 8,413 x **Carat** + 158.1 x **Cut** + 454 x **Clarity**

## Steps to Success
### Step 1 – Understand the data: There are two datasets.
- [**diamonds.csv**](https://github.com/KOdoi-OJ/Predicting-Diamond-Prices/blob/main/datasets/diamonds.csv) contains the data used to build the regression model.
- [**new_diamonds.csv**](https://github.com/KOdoi-OJ/Predicting-Diamond-Prices/blob/main/datasets/new-diamonds.csv) contains the data for the diamonds the company would like to purchase.
![Dataset Preview](https://video.udacity-data.com/topher/2017/February/58a4de9c_data-snapshot/data-snapshot.png)

Both datasets contain carat, cut, and clarity data for each diamond. Only the *diamonds.csv* dataset has prices. You'll be predicting prices for the *new_diamonds.csv* dataset.
- *Carat* represents the weight of the diamond, and is a numerical variable.
- *Cut* represents the quality of the cut of the diamond, and falls into 5 categories: fair, good, very good, ideal, and premium. Each of these categories are represented by a number, 1-5, in the *Cut_Ord* variable.
- *Clarity* represents the internal purity of the diamond, and falls into 8 categories: I1, SI2, SI1, VS1, VS2, VVS2, VVS1, and IF. Each of these categories are represented by a number, 1-8, in the *Clarity_Ord* variable.
- **Note:** Transforming category variables to ordinal variables like this is not always appropriate, but we’ve done it here for simplicity.
### Step 2 – Calculate the predicted price for diamond
For each diamond, plug in the values for each of the variables into the linear model (equation). Then solve the equation to get the estimated, or predicted, diamond price. We suggest using a spreadsheet tool like Excel, Numbers, or Google Sheets. You could also do it in Alteryx and/or Tableau if you already have your license.
### Step 3 - Make a recommendation
Now that you have the predicted price for each diamond, it’s time to calculate the bid price for the whole set. Note: The diamond price that the model predicts represents the final retail price the consumer will pay. The company generally purchases diamonds from distributors at 70% of that price, so your recommended bid price should represent that.
## Project Submission
To complete this project, you will be submitting a file in pdf format that contains the answers to the following questions across three steps.

**Step 1 - Understanding the Model:**
1.	According to the linear model provided, if a diamond is 1 carat heavier than another with the same cut and clarity, how much more would the retail price of the heavier diamond be? Why?
2.	If you were interested in a 1.5 carat diamond with a Very Good cut (represented by a 3 in the model) and a VS2 clarity rating (represented by a 5 in the model), what retail price would the model predict for the diamond?

**Step 2 - Visualize the Data:** Create two scatter plots
- Plot 1 - Plot the data for the diamonds in the database, with carat on the x-axis and price on the y-axis.
- Plot 2 - Plot the data for the diamonds for which you are predicting prices with carat on the x-axis and predicted price on the y-axis.
- Note: You can also plot both sets of data on the same chart in different colors.
- What strikes you about this comparison? After seeing this plot, do you feel confident in the model’s ability to predict prices?
- 
**Step 3 - The Recommendation:** What bid do you recommend for the jewelry company? Please explain how you arrived at that number.
 
## Data
- **diamonds.csv** - contains carat, cut, clarity, and price information for each diamond in the dataset used to build the regression model.
- **new_diamonds.csv** - contains carat, cut, and clarity information for the diamonds the company would like to purchase.

 
# **Replicating Project 1 in Alteryx (Practice Project 1)**
## Background
This section is a practice project that is to assess how ready you are for the actual project that you will submit for review. You'll be going back to the predicting diamond prices project you did for project zero, but this time, you'll be building and validating the model before making the predictions.
## Steps to Success
The steps without descriptions are same as in the First Section, i.e., this section uses the same dataset and related descriptions and explanations.

**Step 1 – Understand the data**

**Step 2 – Build the model:** In project zero, the results were provided, but now you get to calculate them. A few things are different this time around:
- You have more potential predictor variables
- You now know how to use categorical variables, so no need to rely only on ordinal variables.
- When using Alteryx, you do not need to manually create dummy variables before building the model. If you select a categorical variable, like cut or clarity, then Alteryx will automatically create the dummy variables and give you the correct regression output.

**Step 3 – Calculate the predicted price for diamond**

**Step 4 – Make a recommendation**

***Self-Assessment***
Rather than submitting this project, you can self-assess by looking at a sample solution, a solution Alteryx workflow, and/or a detailed walk-through. Do your best to do it on your own, but don't hesitate to use the resources provided when you get stuck.

## Results
The final submission, accepted after review, is [here](https://github.com/KOdoi-OJ/Predicting-Diamond-Prices/blob/main/Kwame%20Odoi%20Otchere%20-%20Predicting%20Diamond%20Prices%20submission.pdf). The other deliverables can also be found here: [predictions for original diamonds](https://github.com/KOdoi-OJ/Predicting-Diamond-Prices/blob/main/datasets%20with%20predictions/diamonds%20with%20predictions.xlsx), [new predictions](https://github.com/KOdoi-OJ/Predicting-Diamond-Prices/blob/main/datasets%20with%20predictions/new-diamonds%20with%20predictions.xlsx), and [Alteryx workflow](https://github.com/KOdoi-OJ/Predicting-Diamond-Prices/blob/main/Practice%20Project%20-%20Predict%20Diamond%20Prices%20with%20Alteryx.yxmd)
## Credits
Credit to Udacity for the materials and the mentors

*This project was completed (with final approval) on February 23, 2022*
