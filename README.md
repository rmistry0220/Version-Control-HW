### Version-Control-HW

In example.py use the following to run the python script in the base environment 

```sh
python app/example.py
```

### Setup for Unemployment Python Script

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
### Usage

Run the unemployment script:
```sh
python app/unemployment_report.py
```