<h1>Stock Exchange Data Analysis</h1>

<h4>DESCRIPTION</h4>
<h5>Objective:</h5>
<p>To use hive features for data engineering or analysis and sharing the actionable insights</p>
<h5>Problem Statement:</h5>
<p>NewYork stock exchange data of seven years, between 2010 to 2016, is captured for 500+ listed companies. The data set comprises of intra-day prices and volume traded for each listed company. The data serves both for machine learning and exploratory analysis projects, to automate the trading process and to predict the next trading-day winners or losers.. The scope of this project is limited to exploratory data analysis.</p>
<h4>Domain:</h4>
<b>BFSI</b>
<h4>Analysis to be done:</h4>
<p> Exploratory analysis to understand how MoM or YoY companies from different sectors or industries and states have progressed in a period of 7 years</p>
<h4>Content:</h4>
<p>This data set contains prices.csv and securities.csv files having the following features:</p>
<h5>Prices.csv:</h5>
<ol>
<li>Date: Trading date</li>
<li>Symbol: Ticker code or listed company code on NY stock exchange</li>
<li>Open: Intra-day opening price for each listed company</li>
<li>Close: Intra-day closing price for each listed company</li>
<li>Low: Intra-day lowest price for each listed company</li>
<li>High: Intra-day highest price for each listed company</li>
<li>Volume: Number of shares traded per day per company</li>
</ol>
<h5>Securities.csv:</h5>
<ol>
<li>1.Ticker_Symbol: Country to which the customer belongs</li>
<li>Security: Legal name of the listed company</li>
<li>Sector: Business vertical of the listed company</li>
<li>Sub_Industry: Business domain of the listed company within a Sector.</li>
<li>Headquarter: Headquarters address</li>
</ol>  
<h4>Steps to perform:</h4>
<p>1) Create a data pipeline using sqoop to pull the data from the table below from MYSQL server into Hive.</p>
<ol type="I">
<li>Stock_prices</li>
<li>Stock_companies</li>
</ol>  
<h5>Check the TABLE description:</h5>
<ul>
<li>TABLE: STOCK_PRICES</li>
<li>TABLE: STOCK_COMPANIES</li>
</ul>  
<p>2) Create a new hive table with the following fields by joining the above two hive tables.</p>
<ul>
<li>Please use appropriate Hive built-in functions for columns (a,b,e and h to l).</li>
<li>Trading_year: Should contain YYYY for each record</li>
<li>Trading_month: Should contain MM or MMM for each record</li>
<li>Symbol: Ticker code</li>
<li>CompanyName: Legal name of the listed company</li>
<li>State: State to be extracted from headquarters value.</li>
<li>Sector: Business vertical of the listed company</li>
<li>Sub_Industry: Business domain of the listed company within a sector</li>
<li>Open: Average of intra-day opening price by month and year for each listed company</li>
<li>Close: Average of intra-day closing price by month and year for each listed company</li>
<li>Low: Average of intra-day lowest price by month and year for each listed company</li>
<li>High: Average of intra-day highest price by month and year for each listed company</li>
<li>Volume: Average of number of shares traded by month and year for each listed company</li>
  </ul>
<h5>DATA ANALYSIS USING HIVE</h5>
 <p>3) Find the top five companies that are good for investment</p>
 <p>4) Show the best-growing industry by each state, having at least two or more industries mapped.</p>
 <p>5) For each sector find the following.</p>
<ol type="I">
<li> Worst year</li>
<li> Best year</li>
<li> Stable year</li>
  </ol>
