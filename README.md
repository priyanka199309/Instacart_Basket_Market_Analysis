# Instacart_Basket_Market_Analysis

Deploying a detailed EDA.

what is Exploratory Data Analysis?
It refers to the critical process of performing initial investigation on data to discover patters, to spot anomalies, to test hypothesis and to check assumptions with the help of summary statistics and graphical representation.
Example: Imagine a group of friends decides to watch a movie they haven’t heard of. There is absolutely no debate about that, it will lead to a state where they find themselves puzzled with lot of questions which needs to be answered to decide. Being a good chieftain the first question they would ask each other, what is the cast and crew of the movie? As a regular practice, they would also watch the trailer of the movie on YouTube. Furthermore, they would find out ratings and reviews the movie has received from the audience.

It is a good practice to understand the data first and try to gather as many insights as possible from it. EDA is all about making sense of data in hand. 





Step 1: Import Python Libraries
To begin with, we need to import all libraries which are required for our analysis, such as Data Loading, Statistical analysis, Visualizations, Data Transformations, Merge and Joins, etc.
Here we are using the following libraries.
•	NumPy-used for Data Manipulation and calculations.
•	Pandas- used for Data Manipulation and calculations.
•	Seaborn-mainly used for graphical representation of the data and findings.
•	Matplotlib- mainly used for graphical representation of the data and findings.  
Here is the link of data:


Step-2:Loading & Reading Datasets:
In this article, Instacart data is being used as an example. In this dataset, we are trying to analyze the on which day usually customers ordered most, or which product is ordered most using Instacart and how EDA focuses on identifying the factors influencing the sale of Instacart. We have stored the data in the DataFrame.
So, we have multiple datasets, so first we will read all the dataset one by one and will try to understand all the datasets.We have Total 7 Datasets, we uploaded all the datasets on JupyterNotebook.



 
First, we need to load the dataset into our notebook. The dataset is typically provided in CSV format and consists of several tables:
•	orders.csv: Information about each order.
•	order_products__prior.csv: Previous order contents for all customers.
•	order_products__train.csv: Training set for the competition.
•	products.csv: Product information.
•	departments.csv: Department information.
•	aisles.csv: Aisle information.

Let's read all the datasets using read_csv() function

Step-3 Analyzing the Data

The main goal of data understanding is to gain general insights about the data, which covers the number of rows and columns, values in the data, datatypes, and Missing values in the dataset.

 


head() will display the top 5 observations of the dataset
tail() will display the bottom 5 observations of the dataset
info() helps to understand the data type and information about data, including the number of records in each column, data having null or not null, Data type, the memory usage of the dataset.


Understanding the Structure
•	Orders Data (orders.csv): Contains information about each order such as user_id, order_id, order_number, order_dow (day of week), order_hour_of_day, etc.
•	Order Products Data (order_products__prior.csv and order_products__train.csv): Contains details about which products were purchased in each order, along with details like add_to_cart_order and reordered.
•	Product Data (products.csv): Provides details about each product including product_id, product_name, aisle_id, and department_id.
•	Department and Aisle Data (departments.csv and aisles.csv): Additional information about departments and aisles.




 





 





 


Check for Duplication
nunique() based on several unique values in each column and the data description, we can identify the continuous and categorical columns in the data. Duplicated data can be handled or removed based on further analysis

 

Missing Values Calculation
isnull() is widely been in all pre-processing steps to identify null values in the data
In our example, data.isnull().sum() is used to get the number of missing records in each column
Exploring Relationships

Now, we will analyze the correlations between variables focusing on order behavior, product details, and customer interactions. for that  we will merge the tables and find the co-relations between all the elements and do our findings for business prospective to help the stakeholders of the company to understand the data more.






