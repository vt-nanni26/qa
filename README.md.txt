Automation & QA Developer Assessment
Task 1
I tested the Conduit (RealWorld Demo) application and identified five issues:

Duplicate account creation allowed with existing credentials.
No confirmation before deleting an article.
Weak password policy allowing one-character passwords.
Invalid email formats accepted during registration.
Long article content causing UI layout breakage.
A root cause analysis was performed for the weak password validation issue.

Task 2
APIs Used
CoinGecko Markets API
CoinGecko Coin Details API
Workflow Logic
Schedule Trigger runs every hour.
HTTP Request retrieves cryptocurrency market data.
JavaScript Code node filters the response to keep the top 5 cryptocurrencies.
Second HTTP Request enriches the data by fetching detailed information about each coin.
Transformation
The workflow extracts important fields such as coin ID, name, symbol, and current price.

Output
The processed data can be extended to email, Telegram, Discord, Slack, or Google Sheets notifications.

Error Handling
The workflow was designed to support n8n execution monitoring and can be extended with Error Trigger and Continue On Fail functionality.