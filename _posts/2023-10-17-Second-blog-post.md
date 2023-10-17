# Exploratory Data Analysis (EDA)

Exploratory Data Analysis is an analysis approach to identify patterns, features, and outliers in data. It is the first step of dealing with data. EDA is not a formal process but rather an art dependent on the problem at hand. In simple terms, it is all about asking questions (a lot of them) and understanding the data through the application of a variety of techniques.  

In this blog post, I will explain my strategy for EDA, specifically how I approach it, and the things I try to look for.

## Overall Goal
My overall goal during any EDA is to understand the data at hand. The process helps me see patterns in data, identify outliers and data gaps, correlate variables, and generate interesting questions.

## Data Context
Prior to any exploratory analysis, I try to understand the context of the data. This helps me formulate relevant questions and the primary purpose of the analysis. I talk to the team that collected the data and ask some simple questions:  
  + purpose of the study/ research
  + data collection method (to identify biases)
  + variables of interest (if any)

## Methods 
I feel graphical summaries are the best tools for exploratory data analysis in general. Based on the type of variable (categorical, quantitative) I am dealing with, I apply different methods. 

### Identify Missing Data
For any type of variable, the first step I do is to get a summary of missing data. This helps make an informed decision if there are any issues in the data set.

### Categorical Varibale
For categorical type variables, I use the following methods to see trends in data:  
  + bar plot: a frequency chart that helps visualize the number of times a categorical variable occurs
  + contingency table or frequency table: gives a count of categorical variables at each level

### Quantitative Varibles
For quantitative variables, I use the following methods:  
  + histogram with kernel density plot (univariate summary): a frequency plot showing the distribution of the numerical variable. This plot gives important information about skewness in data, and symmetry, important information for statistical analyses
  + boxplot (univariate summary): a great way to visualize measures of central tendency, spread, and outliers 
  + scatter plot (multivariate summary): relationship of one variable against another
  + correlation plot or matrix: a plot or matrix showing correlation among different variables

## Things to Watch
I use these tools to look for the following features:  
  + missing data: is the data really missing (for example a voluntary survey) or a data entry issue
  + distribution of variables: skewness, shape. These factors will help us apply appropriate statistical methods for analyses
  + outliers: investigation will help us determine if there it was really an anomaly or there were systematic issues in data collection process
  + correlation among variables
