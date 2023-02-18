# Country's GDP Clustering For Financial Aid
The "Country's GDP Clustering for Financial Aid" is the final project from Basic Data Science class in Sanbercode per February 2022. <br>
The full dataset can not be shared publicly, but it contains 10 features, those are: 
* Country
* Child Mortality
* Export
* Health Cost
* Import
* Income per Capita
* Inflation
* Life Expectancy
* Fertility Rate
* GDP per Capita.

## Context
The Help International is an NGO that focused in reducing poverty. In this case, Help International already fundraised USD 10 million and wants to donate it to some countries.

## Objective
To give recommendation to Help International regarding which countries are eligible to get the donation (with total USD 10 million). <br>
There is a specific criteria that should be fulfilled, it should be indicated by the country's health and socioeconomic.

## Step-by-step
1. See the information of the data, including its type.
2. Define which features are considered health and socioeconomic, which resulted:
* Health: Health cost, child mortality, fertility rate, and life expectancy.
* Socioeconomic: GDP per capita, income per capita, import, export, and inflation.
3. Visualize the correlation among features, to know whether it is positive/negative correlated, or no correlation at all. Especially, between the 'health' and 'socioeconomic' features.
4. **Choose 2 features**:
* Feature that could be represented as socioeconomic is the **GDP per capita**.
* From step 3, there is only 1 feature from health that is not correlated to GDP per capita, which is **Health cost**.
5. Visualize the relation between those 2 through scatterplot and drop outlier (if any).
6. Create clusters with Elbow Method, which resulted into 4 clusters (0, 1, 2, 3).
7. After clustering, there are still some data that overlapped with each others and I decided to create a new parameter, which could be calculated from dividing the 'Health Cost' to 'GDP per capita'. <br>
It means, if the ratio is getting higher, there is a high cost of 'Health' compared to 'GDP per capita' of the country.
