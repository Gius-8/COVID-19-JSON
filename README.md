# COVID-19 JSON Dataset
All data is acquired from the [Johns Hopkins CSSE repository](https://github.com/CSSEGISandData/COVID-19).
The system downloads the daily reports in csv format and converts them to json.

The ***csse_covid_19_daily_reports_csv*** and ***csse_covid_19_daily_reports_json*** folders contain the reports in order by date starting from March 1st. 

Each file is renamed in the format: ***MM-DD-YYYY.csv in UTC***

While the ***most_recent_reports.json*** JSON file contains the most recent data.

You can download the JSON file from this link: 
https://raw.githubusercontent.com/Gius-8/COVID-19-JSON/master/most_recent_reports.json

## JSON example
```
{
    "Reports": [
        {
            "Province/State": "Hubei",
            "Country/Region": "Mainland China",
            "Last Update": "2020-03-04T12:53:03",
            "Confirmed": "67332",
            "Deaths": "2871",
            "Recovered": "38557",
            "Latitude": "30.9756",
            "Longitude": "112.2707"
        },
        ...
}
```
All timestamps are in UTC (GMT+0).

## Update frequency
Once a day.
