# Ratgression
*This is from the final project for the Spring 2025 Econometrics class.*

The "broken windows" theory holds that visible signs of disorder can lead to crime. Does the data support this?

*Ratgression* investigates if complaint types that we presumed would be less susceptible to reverse causality with shootings – like sanitation, infrastructure, and noise rather than violence itself – correlate with increases in reported crimes.

## Project Structure

 - `Ratgression.ipynb`: Main Jupyter notebook containing data import, cleaning, analysis, and regression modeling.

 - `requirements.txt`: List of Python packages required to run the notebook.

 - `.env`: You need to make this file and store your NYC OpenData API token here.

 - Additional CSV or JSON files used for local data processing are provided in the repo or should be downloaded via the notebook.

## Setup
1. Clone the repository:
```
git clone https://github.com/Anantesh-Mohapatra/ratgression.git
cd ratgression
```

2. Install dependencies:

``` pip install -r requirements.txt ```

3. Set up API access:
 - Go to [NYC OpenData](https://data.cityofnewyork.us/profile/edit/developer_settings) to get an API token.
 - Create a .env file in the project root, and paste your API token there in this format:
   - `NYC_OPENDATA_TOKEN=your_api_token_here`

4. Run the notebook:
- Open Ratgression.ipynb in Jupyter Notebook or Jupyter Lab

## Data Sources

311 Service Requests: [NYC OpenData](https://data.cityofnewyork.us/Social-Services/311-Service-Requests-from-2010-to-Present/erm2-nwe9/about_data)

NYPD Crime Complaints: [NYC OpenData](https://data.cityofnewyork.us/Public-Safety/NYPD-Shooting-Incident-Data-Historic-/833y-fsy8/about_data)

Geospatial data: [nycehs's NYC_geography Github repository](https://github.com/nycehs/NYC_geography/blob/master/CD.geo.json)

# *And a message to our professor*
Hi, Professor Manzan. To run our Ratgression code, you must:
- Get an API token from [NYC OpenData](https://data.cityofnewyork.us/profile/edit/developer_settings)
  - Add this API token to a .env file in the same folder you are running the Jupyter notebook in.
- Ensure the attached files are also in the same folder you are running the Jupyter notebook in.
- In the case you don't have one of the packages used in this notebook, running ```pip install -r requirements.txt``` in your terminal will install all the packages used in our code.