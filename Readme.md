### Fintech Case Study

Show a simple table that shows portfolio and fund composition details for each day

#### **Use Case**

1. Use the JSON artifacts generated by the `Portfolio Publisher` and `Fund Compositions` repositories.
2. Fetch historical stock prices for the relevant tickers on each date using an open-source stock price API.
3. Compute and display the value of each fund based on the stock prices and proportions.

1. https://github.com/PruNexus-Developer-Tests/FT-Portfolio-Publisher
2. https://github.com/PruNexus-Developer-Tests/FT-Fund-Compsition

#### **Sample Table**
Here’s an example of the desired table layout:

| Date       | Fund Name | Total Value | Breakdown                       |
|------------|-----------|-------------|---------------------------------|
| 2024-12-20 | Fund A    | $1,200.50   | AAPL: $600.25, GOOG: $600.25   |
| 2024-12-20 | Fund B    | $850.75     | MSFT: $595.53, AMZN: $255.22   |

#### **Steps to Complete**

1. Clone the repositories `Portfolio Publisher` and `Fund Compositions` and generate your own tokens to fetch data from actions.
2. Generate artifacts using their respective GitHub Actions.
3. Use the [Alpha Vantage API](https://www.alphavantage.co/) (or another open-source stock price API of your choice) to fetch stock prices for the relevant tickers on each date. Sign up for a free API key.
4. Calculate the total value of each fund:
   - For each fund, multiply the `units_owned` by the sum of `(stock price * proportion)` for all tickers in the fund.
5. Develop any number of apps or connect any number of platforms to automate the data extraction and modelling and expose an api to a front end.
6. Build a webpage that:
   - Displays the data in a table format as shown above.
7. Write a brief explanation of your approach and any assumptions you made.

#### **To Be Demonstrated**

Develop an end-to-end stack focused on the following areas:

- **Automation:** Automatically extracts and models data.
- **Data Modelling:** Transform and extract data for front-end use.
- **Data Accuracy:** Ensure data validity and precision.
- **Unit Testing:** Write tests to validate data and functions.
- **Error Handling:** Gracefully manage API errors and incomplete data.

#### **To Be Architected or Designed**

Plan and showcase designs for the following areas:

- **Scalability:** Design solutions that can handle increasing data volumes or additional data sources.
- **Security:** Demonstrate secure handling of API keys and sensitive data.
- **Enterprise Integration:** Show how your solution could integrate into existing enterprise systems or workflows.

#### **Submission**

1. Submit your code as a GitHub repository.
2. Include a `README.md` file in your repository with:
   - An overview of your solution.
   - Setup instructions.
   - How to run your code.

Feel free to ask questions or clarify assumptions as needed. Good luck!
