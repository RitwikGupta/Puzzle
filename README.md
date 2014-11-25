# Build a Web API

## 
A Runa customer, AwesomeShoes.com, needs a new report. They've given us their session data, which is a pipe delimited formatted file. Runa also has data stored in a CSV formatted file.  The report should compare the data in the 2 files, and builds a report which shows the discrepancies.

## Requirements
* You need to create a web service, which has a single route, which generates a report as described in the [expected api response](https://github.com/StaplesLabs/code-puzzle/blob/master/expected-api-responses.json).

## API route:
* /runatic/report - route which returns the report data. It takes a parameter `order_by`, which can be any of these 3 values
  * `session-type-desc`         - sort by `session-type` in descending order
  * `order-id-asc`              - sort by `order-id` in ascending order
  * `unit-price-dollars-asc`    - sort by `unit-price-dollars` in ascending order<br />
[This](https://github.com/StaplesLabs/code-puzzle/blob/master/expected-api-responses.json) file has the above 3 use cases.


## Inputs
  * Files located in the resources folder
    * [Merchant Data File](https://github.com/StaplesLabs/code-puzzle/blob/master/resources/merchant_data.psv) is the data from AwesomeShoes.com          
    * [Runa Data File](https://github.com/StaplesLabs/code-puzzle/blob/master/resources/runa_data.csv) is the data stored in Runa's database

## Outputs
Look at this file - [expected api response](https://github.com/StaplesLabs/code-puzzle/blob/master/expected-api-responses.json)
