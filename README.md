# Argo - Onboarding Ticketmaster

This repository is related to the task **"Onboarding Assessment | Ticketmaster"** and it's structured as follows:

```
_assets/
```

### \_assets
This directory stores files to support and facilitate the development of the project.

---

## Task Description:

### Client Scenario
Client Y, a leading force in event management and promotion, is aiming to refine its event strategy, enhance marketing efforts, and boost customer engagement by leveraging detailed analytics from the entertainment sector. Through data obtained from the Ticketmaster Open API, your role is to derive insights on event trends, audience preferences, and venue effectiveness to guide strategic decisions that improve event attendance, increase revenue, and enhance customer satisfaction.

### Objective
Your task involves using the Ticketmaster Open API to extract detailed data on events, venues, ticket sales, and artists. This data will then be transformed, analyzed, and visualized to offer actionable insights. These insights will be depicted through interactive dashboards in Domo, addressing specific business inquiries posed by Client Y.
Data Attributes

The Ticketmaster API grants access to data points such as:
 
* **Event Information:** Name, type (concert, sports, arts & theater), dates, status (on sale, canceled), genre, and subgenre.
* **Venue Details:** Name, location (latitude, longitude, address), capacity, and event schedule.
* **Ticket Sales:** Price ranges, sale dates, available quantities.
* **Artist/Performer Details:** Name, genre, popularity, and event participation history.
(Note: Due to API limitations, customer interactions data will not be included in this analysis.)
 
### Steps
* **Data Extraction:** Develop a Python script for fetching detailed event, venue, ticket sales, and performer data from the Ticketmaster Open API.
* **Data Transformation and Loading:** Process and structure the retrieved data for analysis, then load this data into either Google BigQuery or Snowflake. Design the schema to facilitate advanced analytical queries.
* **Data Analysis in BigQuery:** Execute SQL transformations and analyses within BigQuery or Snowflake to generate datasets that resolve the strategic questions from Client Y, focusing on insights into event performance, audience engagement, and market trends.
* **Visualization in Domo:** Create interactive dashboards in Domo that clearly visualize the analytical findings, providing actionable insights into the dynamics of the entertainment industry.
* **Strategic Recommendations:** Formulate data-driven strategies for Client Y to enhance event selection, marketing initiatives, and customer engagement based on your analytical findings.

### Deliverables
* Python scripts for data extraction from the Ticketmaster Open API.
* BigQuery/Snowflake schema documentation and data loading methodology.
* SQL queries for data analysis within BigQuery/Snowflake.
* Domo dashboards visualizing critical insights.
* Presentation of above materials

### Assessment Criteria
Your work will be evaluated on the efficiency and accuracy of your data extraction and preparation, the depth of your analysis, the innovative and clear presentation of your dashboards in Domo, and the practicality and inventiveness of your strategic recommendations.
 
This project is designed to test your proficiency across the full spectrum of data analytics, from API data extraction and data engineering to analytical thinking and strategic planning, utilizing specific tools (Domo and BigQuery) to provide comprehensive insights for business strategy enhancement in the entertainment and events sector.

### Appendix
* **Ticketmaster API:** https://developer.ticketmaster.com/products-and-docs/apis/getting-started/

### Notes:
* You will need to sign up for a free Ticketmaster account in order to access the APO
* BigQuery/Snowflake has a generous free tier. You will need to create/sign up for a free GCP account to load data into BQ or start a * 30-day trial for Snowflake.
* Domo has a pre-built connector that can pull BigQuery/Snowflake data in for analysis
* You will need to grant Domo access to your GCP/Snowflake account

### A couple of notes...
* Feel free to use whichever data warehouse you are comfortable with. In the past, candidates have used Google BigQuery or Snowflake, as both have generous free tier options to get up and running with no cost to you.
* You will be receiving an email from Domo to set up your account. This is where you will ingest your analytics-ready datasets and build your dashboard(s).
* Although not listed as requirements for this project the following are highly recommended:
    * dbt or SQL Mesh as the transformation layer
    * dlt (data load tool) as the ingestion python package
* You are not expected to host your python script in production. Locally running code is sufficient for this project – we will want to do a code review during your presentation.
* The onboarding document is intentionally vague. Please create a ClickUp Doc and document any assumptions you make so that we can use them to evaluate your decisions. Paste the link to that document as a comment in the Activity section on the right hand side of this task (see screenshot below).
