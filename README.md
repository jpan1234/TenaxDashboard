# Cannabis Market Dashboard for Tenax Strategies
Project to create Massachusetts cannabis industry data dashboard for Tenax Strategies.


The Python script, `api_pull.py`, is designed to interact with a set of APIs provided by the Massachusetts Cannabis Control Commission. It pulls data from various resources and is used to update a Tableau dashboard on a weekly basis.

## Features

1. **MongoDB Connection**: The script establishes a connection with a MongoDB server using a connection string stored in an environment variable. 

2. **API Data Pull**: The script pulls data from a variety of URLs, each corresponding to a different dataset provided by the Massachusetts Cannabis Control Commission. These datasets include information about approved applications, pending applications, agent gender and race, retail sales, and more.

3. **User Agent Rotation**: To avoid potential 403 errors due to too many requests from the same user agent, the script includes a list of user agents and randomly selects one for each request.

## Usage

This script is scheduled to run on a weekly basis to update a Tableau dashboard with the latest data. Ensure that the MongoDB connection string and the last updated date are correctly set in your environment variables before running the script.

## Dependencies

The script depends on several Python libraries, including `json`, `pandas`, `requests`, `random`, `time`, `io`, `os`, `pymongo`, and `beautifulsoup4`. Make sure these are installed in your Python environment before running the script.

## Note

This script is part of a larger system and may not function as expected if run in isolation. Always ensure it is used in its intended context.

## Tableau Dashboard
Using the data scraped from the Cannabis Control Commission Massachusetts, a Tableau dashboard was implemented.

## Visualizations
<img width="1028" alt="image" src="https://github.com/jpan1234/TenaxDashboard/assets/122037319/389d894a-3f42-4c13-8862-d6f6f158a869">

The dashboard has multiple visualizations to help the user track the cannabis market. This includes:

**Distribution of Approved, Pending, and Reopened Applications**
A geographic graph that shows the distributions of approved, pending, and reopened applications for sites to sell cannabis within Massachusetts.

**Yearly Sales in Grams**
Shows the yearly sales of cannabis products in grams. Can be filtered based off of year and product type.

**Top Selling Products**
Shows the top selling products over a range of years that can be filtered. 

**Competitive Pricing Over Time for Grams**
Shows the pricing changes over time for grams of cannabis products. Can be filtered by year and product type. 

## REQUIREMENTS:
Tableau is required to view and interact with this dashboard.


