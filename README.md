# sg-house-prices
Number of house sales and value by quartile

Residential property transactions are recorded by Registers of Scotland. For more information, see https://www.ros.gov.uk/_data/assets/pdffile/0020/3935/StatisticsGuidanceNotes.pdf.

Historical figures include additional coding by the Land Valuation Information Unit at the University of Paisley and Scottish Government. The number of sales, median price and lower quartile price are based on second hand and new build sales that are recorded/registered whether they are cash purchases or funded by mortgages. The mean price is based on new build and second hand sales between £20,000 and £1,000,000.

Includes two datasets on statistics.gov.scot
* [House Prices](http://statistics.gov.scot/data/house-sales-prices)
* [House Sales](http://statistics.gov.scot/data/house-sales)

Reference areas extracted: Data Zones 2001.

## License

Data is licensed under the Open Government License: http://www.nationalarchives.gov.uk/doc/open-government-licence/version/2/

## Requirements

- NodeJS
- npm

## Installation

Clone the repository

```
git clone https://github.com/EdinburghCityScope/sg-house-prices.git
```

Install npm dependencies

```
cd sg-house-prices
npm install
```

Run the API (from the sg-house-prices directory)

```
node .
```

Converting the extracted data into loopback data.

```
node scripts/featureCollectionToLoopbackJson.js
```

Re-build data files from the statistics.gov.scot API

```
node scripts/build-data.js
```
