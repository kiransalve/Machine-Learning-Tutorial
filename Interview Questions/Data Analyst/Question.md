Question 1

Can you please introduce yourself and tell me why you’re applying for this Data Analyst role at Capgemini?

Answer 1

"Hello, I’m Kiran. I’ve been working for the past 7 years in the Sales and Marketing department of a manufacturing company,
mainly as an Sales Analyst with a strong focus on data cleaning, data formating, data modeling, data analysis and data visualization.

Over time, I’ve naturally grown into a data analyst role by handling responsibilities like sales tracking, 
forecast vs actual analysis, marketing scheme achievement reporting, incentive calculation 
and even financial tasks like outstanding reports, DSO reports, freight analysis and Product cost analysis

I work daily with tools like Power BI,pivot tables and MySQL to prepare dashboards and reports that support both sales and finance teams. 

One of the best things I have done is automating our weekly zonal sales performance dashboard using Power BI, 
which gave our Zonal Heads real-time visibility into sales performance and helped them take quicker decisions.
It have HQ wise data like budget vs actual sales, pending and finance hold orders, current month dificit, ytd dificit, collection vs outstanding and inventory lying with distributor end.

I’m now have experince to work with cross functional teams like purchase, dispatch, finance, accounts teams and also work 
independantly on any given project, currently I am trying to connect our dashboard to directly to SAP Hana instead of MySQL.

I’m applying for this Data Analyst role at Capgemini because I want to take the next step in 
my career — work on more advanced data projects, collaborate with diverse teams, and learn from experienced professionals in a structured, 
fast-paced environment of Capgemini.
I know Capgemini is a leader in digital transformation and analytics, and I’m excited to contribute my domain experience, 
strong reporting skills, and eagerness to grow into more advanced analytics and AI-driven roles over time"


Question 2

Can you tell about your latest project with KPI, data source and how did you develope it.

Answer 2

"Yes, I recently worked on a Sales Forecasting Project to help our sales and production planning teams estimate next month's sales based on historical trends.

The goal was to forecast monthly product-wise sales for better production planning and inventory control — especially for fast-moving poultry supplements where stockouts were frequent and dairy product where lead time is more because raw material come from china so understockcing scenarios happens.

I use data source as MySQL, and fetched last 24 months sales register, and joines by region and product group and then I grouped this
into monthly productwise sales using SQL 

KPI for this included - Next Month Qty, Forecast Accuracy (MAPE), Top 10 and Bottom 10 Products with most deviation

also we monitor last month forecast vs sales.

I have used Python - Pandas, Profet, Scikit-learn , Power BI to present the forecast alongside actuals and SQL for data extraction and aggregation

I aggregated monthly sales using SQL (GROUP BY Month, Item Code) and cleaned missing/inconsistent entries.

I used the Prophet model (by Facebook) for each top-selling product to capture seasonality and trend

For comparison, I also built a simple moving average and linear regression model.

I evaluated models using MAPE and selected the best-performing one for each product.

I stored the forecasted numbers and used Power BI to compare them visually with actuals, with variance alerts.

The forecast helped our production and dispatch team pre-plan for high-demand products, especially before peak seasons. 
We saw a reduction in stockouts by ~20% and improved coordination between sales and supply chain.

It also helped Zonal Managers proactively push schemes for under-forecasted products.
This project gave me hands-on experience with time series models, and I’m now exploring ways to scale it using Python MLOPS for automatic monthly updates."

Question 3

What schema did you follow in your sales forecasting project and why?

Answer 3

In my sales forecasting project, I followed a Star Schema design.

The core idea was to keep the structure simple, performant, and easily scalable for both Power BI and modeling in Python.

We had one central fact table — fact_sales_monthly — which stored monthly aggregated sales and forecast data like qty_sold, amount, forecast_qty, and forecast_amount.

Around this, we built multiple dimension tables like 

dim_date to manage fiscal months and date hierarchies,

dim_product for product-level details like brand and category,

dim_region for mapping zone, region, and HQ,

and dim_forecast_model to track metadata like model type and forecast accuracy (MAPE, RMSE).

I chose the Star Schema because it reduces the number of joins during query execution, which is great for Power BI performance and easier for business users to understand. It also works well with DAX and time-series forecasting pipelines in Python — since everything is cleanly connected to the fact table.

Compared to a Snowflake schema, the Star Schema made the data model more readable, and the performance gain was noticeable — especially when slicing sales or forecasts by region, product, or time.

This structure helped me maintain both reporting efficiency and modeling flexibility as the project scaled."

