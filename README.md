# Hypothesis Testing in Business Analytics using Python  

## 📝 __Overview__  
This project explores a suite of statistical hypothesis tests, encompassing both parametric and non-parametric methods, to evaluate differences between groups, relationships between variables, and distribution characteristics.  
### __Statistical Tests Applied__  
| Parametric Tests | Non-Parametric Tests |
|------------------|----------------------|
| Two-Sample T-Test (Independent Groups) | 	Mann-Whitney U Test |
| Paired T-Test (Before vs. After Campaign) | 	Wilcoxon Signed-Rank Test |
| One-Way ANOVA | Kruskal-Wallis H Test |
| Pearson Correlation Coefficient | 	Spearman Rank Correlation Coefficient |
|  | Chi-Square Test of Independence |
|  | Chi-Square Goodness-of-Fit Test |  
  
Each test is applied considering its assumptions and conditions of validity, supported by preliminary checks such as the __Shapiro-Wilk test__ for normality and __Levene’s test__ for homogeneity of variances.  
The visual representation of data through histograms, Q-Q plots and scatter plots facilitates a clearer understanding of the underlying distributions and assists in the selection of appropriate statistical techniques.  
The dataset used in this study was synthetically generated to simulate realistic sales and regional data patterns. Coding was conducted using Google Colab, a cloud-based Python environment that allows seamless integration with Google Drive and simplifies code execution and data handling. Jupyter Notebook could also be used as an alternative.    

## __📂 Contents__  
| File Name | File Type | Description |
|-----------|-----------|-------------|
| README | MD | Read this before anything else |
| sales_data | CSV | Dataset generated for analysis |
| Code_Hypothesis_Tests_in_Python | IPYNB | Python Notebook |
  
## __▶️ How to Execute the Program__
Before executing the program, download the IPYNB file (Code_Hypothesis_Tests_in_Python) from this repository. Afterwards, follow these steps:  
### If you are using Google Colab:  
•	Open a browser and go to https://colab.research.google.com.  
•	Click on File > Upload Notebook.  
•	Select and open the downloaded IPYNB file.  
•	Click on the run button adjacent to each code snippet to run the code.  
### If you are using Jupyter Notebook:  
•	If you don’t have Anaconda or Jupyter Notebook installed, visit: https://www.anaconda.com and download the installer appropriate for your OS.  
•	After downloading, double-click on the downloaded file and follow the on-screen instructions to complete the installation process.  
•	Locate and run the program ‘Anaconda Prompt’.  
•	Run Jupyter Notebook after navigating to the folder containing the downloaded IPYNB file. For instance, if the files are located in a folder called PythonCode in Local Disk (D:), then you have to run _D:\PythonCode>jupyter notebook_.  
•	After opening the IPYNB file, select the code snippets and click on Run to run the code.  
  
## 🔍 __Observation__  
__Dataset Summary:__ The dataset consists of 360 entries across 8 columns, including region, campaign_type, before_sales, after_sales, ad_spend, and revenue, allowing for comprehensive statistical analysis of marketing effectiveness.  

__Notable Statistical Test Insights:__  

    ✅ Paired t-test showed a significant difference between before and after sales (p < 0.000001), confirming the effectiveness of campaigns.  

    ❌ Independent t-test found no significant revenue difference between Asia and Europe (p = 0.8708).  

    ❌ One-way ANOVA revealed no significant revenue variation among Email, Social Media, and TV campaigns (p = 0.5067).  

    ❌ Pearson Correlation showed no significant linear relationship between ad spend and revenue; a non-parametric alternative may be better due to non-linearity.  

    ❌ Chi-square test of independence indicated no association between gender and email open rates.  

    ✅ Chi-square goodness-of-fit test showed that campaign types are not equally distributed, indicating intentional or skewed targeting.  

These observations help in refining marketing strategies and choosing appropriate statistical methods for deeper insights.  
 
## 📌 __Things to Keep in Mind__  
* For all the tests conducted, the level of significance is taken to be 5% as it is used most commonly.
* Ensure your data doesn't contain NaN values when performing tests or plotting.  
* Modify the file path if you're reading the dataset from your own Drive in Colab.  
