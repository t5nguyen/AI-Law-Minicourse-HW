# AI-Law-Minicourse-HW
## Supreme Court Topic Modeling
### Step 1
> In this step, requests for data is being run using Beautiful Soup, specifically, Supreme Court rulings from 1760 thorugh 2018 is being pulled directly from the CaseLaw website. The results are returned ins a data table which includes as columns, case url and docket. The search results in 23,393 cases. 
### Step 2
> In this step, the 23,393 opinions gathered from Step 1 are broken down into three smaller frames to prevent CaseLaw from blocking the request. The first contains the first 5,000 opinions, the second the next 10,000, and the final the remaining 8,268. Within each group, the case name is scraped and "pickled" (or saved). Once all three are scraped for the case names, they're then recompiled and saved as a whole project. 
### Step 3
> In this third step, the opinions are processed to remove stopwords and to lemmatize. Packages of common English stop words are imported using the sklearn.feature_extraction module and then additional stopwords are created by assigning categories of words, including names (male and female), case names, and state names. To lemmatize words, we define separators ("\r", "\n", and more). This is also applied to the stopwords list created. The resulting case list/information is then "pickled", or saved, for later use. 
### Step 4
> In this next step, we go through different methods for topic modeling the Supreme Court cases extracted in the previous steps to find the best model to use: 
>> 1. Latent Dirchlet Allocation Model;
>> 2. Latent Semantic Analysis; and
>> 3. NMF Model. 
### Step 5
> In this final step, we apply the third model, NMF Model, to the data frame.
## Tensor Flow 
> I was able to launch an empty (Python) kernel in my repository, but had difficulty importing Tensorflow.
