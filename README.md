# House Rocket Insights Project
The goal of this project is to create insights through data analysis and manipulation to help the decision making of the Business Team of a fictional company (House Rocket)
 
## 1 - Business Problem.

### 1.1 - Description
House Rocket is a property purchase and sales company (fictional).

With that in mind, the purpose of this project is to create insights through data analysis to help the company find the best opportunities. So, the business problem is to choose the best properties to buy so that the company can sell for a bigger price and make profits with it. 

The dataset used in this project comes from the official public records of home sales in the King County area, Washington State.

[Dataset from Kaggle](https://www.kaggle.com/harlfoxem/housesalesprediction)

### 1.2 - Business Questions
 1. What properties should House Rocket buy and at what price?
 2. What is the best moment to sell the bought properties and for what price?

### 1.3 - Business Understanding
**Final Product:**
 - Report with property purchase suggestions with price recomendation;
 - Report with property selling suggestions with price recomendation;
 - Insights to help decide which property should be more interesting for the business.
 - A Cloud Application with interactive dashboards, maps and dataframes.

## 2 - Business assumptions.
- Every property is available for buying, independently of any metric (including price);
- Properties with condition 2 or less are considered not in good condition for purchase;
- Seasons are separeted in 2: Summer (June to November) and Winter (December to May);
- Seasons are considered an affecting metric of price;
- Few data cleaning was made.

## 3 - Solution Planning
- **Buying and Selling Report:**

 **Buying Plan:**

 **Step I** - Collect data from Kaggle;
 
 **Step II** - Group the properties by zipcode (region);
 
 **Step III** - Find the price median by zipcode (market price metric);
 
 **Step IV** - Suggest buying the properties with prices below the market price metric that are in good conditions.
 
 **Step V** - Create a Excel file with all the buying and selling results
 
 
 **Selling Plan:**
 
 **Step I** - Group the properties by season (summer or winter) from its date of post;
 
 **Step II** - Find the price median for each region (zipcode) in each season (summer or winter);
 
 **Step III** - Suggest selling the properties above its zipcode-season-median with a 10% profit margin;
 
 **Step IV** - Suggest selling the properties below its zipcode-season-median with a 30% profit margin.
 
 - **Insights Plan:**

 **Step I** - Make a data analysis based on the hypotesis already made;
 
 **Step II** - Mark them as True or False;
 
 **Step III** - Explain the results obtained for better data understanding.
 
## 4 - Top 5 Business Insights.
**Hypothesis 01:**
Water view properties are, at least, 20% more expensive, on avarege.
**TRUE:** Properties with water view are 212.63% more expensive, on avarege.

|    |   waterfront |   buying_price_mean |
|---:|-------------:|--------------------:|
|  0 |            0 |    531558.54           |
|  1 |            1 |         1661876.02 |

**Hypothesis 02:**
Properties built before 1955 are more than 50% cheaper, on avarege.
**FALSE**: The properties built before 1955 are, actually, 4.46% more expensive, on avarage.

|    |   yr_built |   buying_price |
|---:|-----------:|---------------:|
| 53 |       1953 |         490423 |
| 46 |       1946 |         524641 |
| 25 |       1925 |         607219 |
| 28 |       1928 |         621714 |
| 32 |       1932 |         458409 |
|  5 |       1905 |         752978 |
| 50 |       1950 |         490506 |
| 51 |       1951 |         545029 |
| 52 |       1952 |         530437 |
| 10 |       1910 |         671536 |

**Hypothesis 03:**
properties without a basement have a total area, at least, 40% larger than properties with basement, on avarage.
**FALSE**: Properties without basement are 18.41% larger than the ones with basement, on avarage.

|    | has_basement   |   sqft_lot_mean |
|---:|:---------------|----------------:|
|  0 | False          |         16284.2 |
|  1 | True           |         13287.2 |

**Hypothesis 04:**
The property price growth YoY (Year over Year) is more than 10%.
**FALSE**: The price percentage growth of 2015 over 2014 is 0.52%.

![2014 and 2015 Buying Price Means](barplot_hypothesis_04.png)

**Hypothesis 05:**
Properties with 3 bathrooms have a price growth of more than 15% per month.
**FALSE**: Properties with 3 bathrooms have a price growth of 0.32% per month, on avarage.

![Growth Percentage Over The Months (Month over Month)](lineplot_hypothesis_05_correct.png)

## 5 - Tools used
 - Python 3.9.7;
 - PyCharm;
 - Jupyter Notebook;
 - Excel.

## 6 - Financial Results for the Company
--
## 7 - Conclusion
--
## 8 - Next Steps
- **Cloud Application Creation Plan:**
 
 **Step I** - Get the address using a Geopy (Python library) tool called Nominatim, which can find the nearest address given the latitude and longitude 
 
 **Step II** - Create a document called App.py and develop a application with interactive filters for dashboards using Streamlit Python library;
 
 **Step III** - Deploy the application at Heroku. (Heroku is a cloud platform as a service that supports multiple programming languages.)
