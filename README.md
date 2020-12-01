# DataSciencePreReq-EDA

This Repo shows quite an Exhaustive Approach to "Exploratory Data Analysis" for a consumer finance company which specialises in lending various types of loans to urban customers 

When the company receives a loan application, the company has to decide for loan approval based on the applicant’s profile. Two types of risks are associated with the bank’s decision:
 - If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company

 - If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company.

 
The data contains the information about the loan application at the time of applying for the loan. It contains two types of scenarios:
 - The client with payment difficulties: he/she had late payment more than X days on at least one of the first Y instalments of the loan in the sample,

 - All other cases: All other cases when the payment is paid on time.
 

When a client applies for a loan, there are four types of decisions that could be taken by the client/company:

 - Approved: The Company has approved loan Application

 - Cancelled: The client cancelled the application sometime during approval. Either the client changed her/his mind about the loan or in some cases due to a higher risk of the client he received bad pricing which he did not want.

 - Refused: The company had rejected the loan (because the client does not meet their requirements etc.).

 - Unused offer:  Loan has been cancelled by the client but on different stages of the process.

Here EDA is done to understand how consumer attributes and loan attributes that influence the tendency of default.


The Technical Take-aways from this exercise:

### A typical process or method followed in EDA includes:

- Reading and Inspection of Data
    - The size, shape, the data type, the column names, the multiple sources of data
    - Understanding how many are categorical and continuous variables
- Cleaning the data
    - Dropping columns that may not mean much to the analysis
    - Treating  missing and NULL values
        - Dropping high NULL value columns
        - Deciding to impute the rest (with mean, median, mode etc.)
        - Deciding not to impute and drop those rows, if few, where it makes sense
    - Treating Outliers
        -Understanding outlier and dropping, pruning or replacing with meaningful values
- Creating meaningful new vairbales through Binning
- Creating new convenience columsn esp with dates to durations
#### Data Analysis
- Checking the imbalance in Data
- Univariate Analysis
    - For Catagorical Variables (typically bar charts)
    - For binned Variables
    - For Continuous Variables (typically box plots or line graphs/dist plots)
- Bivariate Analysis
    - Continuous-Continuous Variables (heatmaps and pair plots)
    - Continuous - Categorical Variables (Hued Box plots)
    - Categorical - Categorical Variables (bar plots)
- Check for correlations between varibles and target variable (heatmap, pair plot)

At each of these levels, you can derive insights about what really impacts the target variable and that should help in certain hypothesis and decision on the ML solution.
    
    