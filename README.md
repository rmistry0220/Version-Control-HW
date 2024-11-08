### Version-Control-HW

In example.py use the following to run the python script in the base environment 

```sh
python app/example.py
```

### Setup for Unemployment and Stocks Python Script

Create and activate a virtual environment (first time only):
```sh
conda create -n reports-env-2024-hw python=3.10
```

Activate the environment (whenever you come back to this):
```sh
conda activate reports-env-2024
```

Install packages
```sh
pip install -r requirements.txt
```

Obtain an API Key from AlphaVantage.
Create a ".env" file and add contents like the following (using your own AlphaVantage API Key):
```sh
# this is the ".env" file:
ALPHAVANTAGE_API_KEY="..."
```

### Email Setup
Create a Mailgun account with your business or university email address (i.e. MAILGUN_SENDER_ADDRESS). 

Click the verification link sent to that address.

Login. Find and click the nav link about "Sending" email. From the domains page, note the sandbox domain provided to you by default (i.e. MAILGUN_DOMAIN like "sandbox-xyz.mailgun.org").

Find and click on API Key settings link on bottom right, then on the API Keys page, scroll down and click the button to create a new API Key (i.e. MAILGUN_API_KEY).

Before proceeding, set these credentials in the .env file (MAILGUN_SENDER_ADDRESS, MAILGUN_DOMAIN , and MAILGUN_API_KEY).
```sh
# this is the ".env" file:
MAILGUN_API_KEY="..."
MAILGUN_DOMAIN="...."
MAILGUN_SENDER_ADDRESS="..."
```

### Usage

Run the unemployment script:
```sh
python app/unemployment_report.py
```

Run the stocks script:
```sh
python app/stocks_report.py
```

Run the email sending script:
```sh
python app/email_service.py
```