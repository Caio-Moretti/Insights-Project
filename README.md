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
**1. Final Product:**
 - Report with property purchase suggestions with price recomendation.
 - Report with property selling suggestions with price recomendation.

**2. Tools used:**
 - Python 3.9.7;
 - PyCharm;
 - Jupyter Notebook.

**3. Process:**

 **Buying Plan:**

 **I** - Collect data from Kaggle;
 
 **II** - Group the properties by zipcode (region);
 
 **III** - Find the price median by zipcode (market price metric);
 
 **IV** - Suggest buying the properties with prices below the market price metric that are in good conditions.
 
 
 **Selling Plan:**
 
 **I** - Group the properties by season (summer or winter) from its date of post;
 
 **II** - Find the price median for each region (zipcode) in each season (summer or winter);
 
 **III** - Suggest selling the properties above its zipcode-season-median with a 10% profit margin;
 
 **IV** - Suggest selling the properties below its zipcode-season-median with a 30% profit margin.

### 1.4 - Data Exploration
- Make a Big Data Analysis
- Find Insights for the Business Team

## 2 - Business assumptions.

## 3 - Top 5 Business Insights.
**Hypotesis 01:**
Water view properties are, at least, 20% more expensive, on avarege.

**Hypotesis 02:**
Properties built before 1955 are more than 50% cheaper, on avarege.

**Hypotesis 03:**
properties without a basement have a total area, at least, 40% larger than properties with basement, on avarage.

**Hypotesis 04:**
The property price growth YoY (Year over Year) is more than 10%.

**Hypotesis 05:**
Properties with 3 bathrooms have a price growth of more than 15% per month.

## 4 - Financial Results for the Company
--
## 5 - Conclusion
--
## 6 - Next Steps
--
