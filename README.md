# Popsical API Doc

http://developers.popsical.com

`/dist` - swagger-ui fetches http://developers.popsical.com/v1/api.json

## Developers

Edit v1/api.yml, v2/api.yml to add/update endpoint specification.

## Setup

`bundle install`


## Usage

1. Edit `v1/api.yml` or `v2/api.yml`. Use swagger 2.0 yaml syntax

2. `rake build` - this will generate v1/api.json and v2/api.json

3. `rake publish` - deploy to s3 bucket