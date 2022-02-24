# Analyze Supermarket Data Across the Country - Company XYZ
Company XYZ owns a nationwide supermarket chain. Each of the country's major branches, located in Lagos, Abuja, and Port Harcourt, kept track of sales for three months. The goal of this project is to assist the company in better understanding sales trends and determining its growth as supermarket competition keeps growing.

# The phases of the project and a summary of the tasks that have been done
The phases of the project invovles:
1. Defining the question
The following questions were created in order to assess which data features would be most useful in solving the problem.
What business issue am I attempting to address?
What makes this such a high priority for the organization right now?
What can I do to make this as simple as possible?
What am I hoping to achieve?

Collecting the data
The files included sales data from three distinct branches in Lagos, Abuja, and Port Harcourt over a three-month period. The feature information is the same in each data file from the branches; see the feature explanation below.
Invoice ID: Customer Identification number
Branch: Supermarket Branch across the country (A, B, C)
A - Lagos Branch
B - Abuja Branch
C - Port Harcourt Branch
City: Supermarket Location
Customer Type: Type of customers, Members - Returning customer with membership card, Normal - Customer without membership (could be returning, first-time or walk-in customer)
Gender: Customer Gender Information
Product line: Product categorization groups - Electronic accessories, Fashion accessories, Food and beverages, Health and beauty, Home and lifestyle, Sports and travel
Unit Price: Price of each product in Naira
Quantity: Number of products purchased by customer
Tax: 5% tax fee for customer buying
Total: Total price including tax
Date: Date of purchase (Supermarket Record available from January 2019 to March 2019)
Time: Purchase time (Supermarket Hours - 10am to 9pm)
Payment: Payment used by customer for purchase (3 methods are available – Cash, Card and Epay)
COGS: Cost of goods sold
Gross margin percentage: Gross margin percentage
Gross income: Gross income
Rating: Customer Satisfaction rating on their overall shopping experience (On a scale of 1 to 10)

Cleaning the data
The following steps are included in the data cleaning process when preparing data for analysis:
i. Data relevance
The data sets given were useful in answering the questions and analyzing them.
ii. Data Consistency
The data sets that were supplied were consistent.
iii. Data Exploration
In the datasets, there were no duplicate or null values.
iv. Data correctness
Converted the date column to datetime. All other functionalities were appropriately given.
v. Feature development
Extraction of the Day, Month, Year, and Hour features from the Date feature was done.

Analyzing the data
After successful data cleaning, data analysis was carried out by doing analysis on unique values in columns and aggregation with grouping.

Visualize and Sharing results
After a successful analysis, the following visualization was created through:
i. Effective use of countplot to discover which branch has the best sales record.
ii. Use of countplot to find the most popular payment method and the city with the most sales.
iii. Use of countplot to find the greatest and lowest selling product lines.
iv. The payment channel utilized by the majority of clients to purchase for each product line.

# Insights
The following insights where derived:
i. The city with the highest total gross income is Port Harcourt, having a total gross income of #13268244.78, with a difference of #524524.14 to the city with the lowest gross income, Abuja.

ii. The city with the highest total Unit price is Lagos, having a total Unit price of #46936234.8, with a difference of #369457.2 to the city with the lowest Unit price, Abuja.

iii. The city with the highest total Quantity is Lagos, having a total Quantity of 13013, with a difference of 273 to the city with the lowest Quantity, Abuja.

iv. The highest sold product line is Fashion accessories and the lowest sold product line is Health and beauty

v. Payment channel used by each product line.
*The payment channel used by most customer to pay for Health and beauty products is Epay.
*The payment channel used by most customer to pay for Home and lifestyle products is Epay.
*The payment channel used by most customer to pay for Sports and travel products is Cash.
*The payment channel used by most customer to pay for Electronic accessories products is Cash.
*The payment channel used by most customer to pay for Food and beverages products is Card.
*The payment channel used by most customer to pay for Fashion accessories products is Epay.

vi. The Payment channel for each branch.
*The Card payment is most used in Abuja Branch.
*The Epay payment is most used in Lagos Branch.
*The Cash payment is most used in Port Harcourt Branch.

vii. Branch 'B' (Abuja Branch) has 50% of it's ratings below 7 while branches 'A' (Lagos Branch) and 'C' (Port Harcourt Branch) have 50% of their ratings above 7. Hence branch 'B' has the lowest ratings.

viii. The gender type effect on kind of products being purchased at the supermarket.
    1. Food and beverages:
	The top 50% of the females purchased more quantities of food and beverages when compared to the top 50% of the males.
	The top 50% of the females spends over #110,000 on food and beverages while the top 50% of the males over #75,000.
	The top 25% of the females spends approximately over #200,000 while the top 25% of the males over #150,000.
Hence, this clearly states that the females have higher purchasing power (ie buys more quantities and spend more) on food and beverages when compared to the male.


   2. Fashion accessories:
	The top 50% of the females purchased more quantities of fashion accessories when compared to the top 50% of males.
	The top 50% of the females spends over #100,000 on fashion accessories while the top 50% of the males over #70,000.
Hence, this clearly states that the females have higher purchasing power (ie buys more quantities and spend more) on fashion accessories when compared to the male.


   3. Electronic accessories:
	The top 50% of the females purchased approximalely equal quantities of electronic accessories when compared to the top 50% of males.
	The top 50% of the females spends over #90,000 on electronic accessories while the top 50% of the males over #80,000.
Hence, this clearly states that both the females and males have approximately equal purchasing power (ie buys same quantities and spend same amount) on electronic accessories.


   4. Sport and travel:
	The top 50% of the females potrays approximalely equal needs on sport and travel when compared to the top 50% of males.
	The top 50% of the females spends over #85,000 on sport and travel while the top 50% of the males over #110,000.
Hence, this clearly states that both the females and males have approximately equal purchasing power (mainly in quantity ) on sport and travel, however the males spends a little more.


   5. Home and lifestyle:
	The top 50% of the females potrays more needs on home and lifestyle when compared to the top 50% of males.
	The top 50% of the females spends over #120,000 on home and lifestyle while the top 50% of the males over #80,000.
Hence, this clearly states that the females have higher purchasing power (ie buys more quantities and spend more) on home and lifestyle when compared to the male.


   6. Health and beauty:
	The top 50% of the females purchased less quantities of health and beauty products when compared to the top 50% of the males.
	The top 50% of the females spends over #90,000 on health and beauty while the top 50% of the males over #100,000.
	The top 25% of the females spends over #160,000 on health and beauty while the top 25% of the males over #190,000.
Hence, this clearly states that the males have higher purchasing power (ie buys more quantities and spend more) on food and beverges when compared to the female.

vix. The interaction of Unit price on the Quantity of goods purchased.
    From catplot, the following insights can be established
	The mean of the Unit price for each product line increased in the following order:
	Electronic accessories->Health and beauty->Home and lifestyle->Food and beverages->Sports and travel->Fashion accessories
	The mean of the product's quantity for each product line increased in the following order:
	Fashion accessories->Food and beverages->Sports and travel->Health and beauty->Home and lifestyle->Electronic accessories
    Hence, Electronic accessories product line has the lowest mean price of product but the highest mean of product quantity purchase by customers. Also the Fashion accessories product line has the highest mean price of product but the lowest mean of product quantity purchased by customers


# Future Work
To gain further insight from the dataset, future work will focus on doing analysis on the Time, Date, and extracted Day, Month, Year, and Hour features.


# Standout Section
The code was done in a simple and clear manner.
The to frame() method was used to make the output more visible.
To provide understandable outputs, format techniques and escape characters (such as \, \n, and \t) were used.
In order to assure a user-friendly display, more parameters were supplied into the seaborn plotting methods.
The association between Unit price, Quantity, and Total price was shown using a Seaborn heatmap graphic.


# Executive Summary.
The Abuja branch had the lowest gross income, unit price, and number of items purchased by clients among the three (3) locations spread across the country. It's possible that this is the outcome of the branch's poor customer service. As a result, the Abuja branch had the lowest rating among the three (3) branches. As a consequence, greater attention should be paid to this branch in order to improve customer satisfaction, which would boost gross revenue and the number of items purchased by customers.

Furthermore, card payments are the most often reported transaction in Abuja, Epay payments in Lagos, and cash payments in Port Harcourt. As a result, it is critical to guarantee that these payment methods are consistently available to their respective branches, as this may be perceived as the preferable way. Customers prefer Epay as a method of payment in the least sold but high quantity sold product lines, such as Health and beauty products and Home and lifestyle products, as well as the most popular product line, Fashion accessories products, so the steady availability of this method of payment in these sections of the product line is also crucial.

Additionally, as compared to male consumers, female customers have greater purchasing power in terms of spending and acquiring larger quantities of products in the food and beverage, fashion accessories, and home and lifestyle product lines. Male clients, on the other hand, tend to spend and buy more in the health and beauty product line.

Finally, if changes are done based on the information provided, the company will be able to better serve its consumers and flourish, despite the increasing supermarket competition.
