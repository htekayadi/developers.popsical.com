# Popsical API Doc

http://developers.popsical.com

`/dist` - swagger-ui fetches http://developers.popsical.com/v1/api.json

## Developers

Edit api.yml to add/update endpoint specification.

## Setup

`bundle install`

## Steps to deploy

1. Edit `v1/api.yml`. Use swagger 2.0 yaml syntax

2. Generate json `api.json` with `rake build`.

3. Upload `api.json` to s3 developers.popsical.com

# TODO

rake task for actual deployment to s3 bucket