# COVID-19 JSON Dataset
All data is acquired from the [Johns Hopkins CSSE repository](https://github.com/CSSEGISandData/COVID-19) and [pcm-dpc](https://github.com/pcm-dpc/COVID-19).  
The system downloads the daily reports in csv format and converts them to json.

The ***csse_covid_19_daily_reports_csv*** and ***csse_covid_19_daily_reports_json*** folders contain the reports in order by date starting from March 1st. 

Each file is renamed in the format: ***MM-DD-YYYY.csv in UTC*** and ***MM-DD-YYYY_italy.csv in UTC***

The ***most_recent_reports.json*** JSON file contains the world most recent data.  
While the ***italy_most_recent_reports.json*** JSON file contains the most recent data in Italy.

You can download the JSON file from this link:   
https://raw.githubusercontent.com/Gius-8/COVID-19-JSON/master/most_recent_reports.json

https://raw.githubusercontent.com/Gius-8/COVID-19-JSON/master/italy_most_recent_reports.json

## JSON world example
```
{
    "Reports": [
        {
            "Province_State": "Hubei",
            "Country_Region": "Mainland China",
            "Last_Update": "2020-03-04T12:53:03",
            "Confirmed": "67332",
            "Deaths": "2871",
            "Recovered": "38557",
            "Latitude": "30.9756",
            "Longitude": "112.2707"
        },
        ...
    ]
}
```
All timestamps are in UTC (GMT+0).

## JSON Italy example
```
{
    "Reports": [
        {
            "last_update": "2020-03-05T18:21:43",
            "latitude": "45.657581",
            "longitude": "9.963600",
            "region": "Lombardia",
            "hospitalized": "877",
            "intensive_care": "209",
            "home_isolation": "411",
            "currently_positive": "1497",
            "recovered": "250",
            "deaths": "73",
            "totals_confirmed": "1820",
            "swabs": "12138"
        },
        ...
    ]
}
```

## Update frequency
Once a day.
