# AI-Law-Minicourse-HW
## Supreme Court Topic Modeling
### Step 1
> In this step, requests for data is being run using Beautiful Soup, specifically, Supreme Court rulings from 1760 thorugh 2018 is being pulled directly from the CaseLaw website. The results are returned ins a data table which includes as columns, case url and docket. The search results in 23,393 cases. 
### Step 2
> In this step, the 23,393 opinions gathered from Step 1 are broken down into three smaller frames to prevent CaseLaw from blocking the request. The first contains the first 5,000 opinions, the second the next 10,000, and the final the remaining 8,268. Within each group, the case name is then scaped from information and placed into the original data table containing all cases originally pulled. This table now includes the case url, docket, year, and case title. 
### Step 3
> In this third step, the opinions are processed to remove stopwords and to lemmatize. Packages of common English stop words are imported using the sklearn.feature_extraction module and then additional stopwords are created by assigning categories of words, including names (male and female), case anmes, and state names. To lemmatize words, we define separators ("\r", "\n", and more). This is also applied to the stopwords list created. 
### Step 4
>
### Step 5
>
