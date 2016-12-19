# Popsical API Doc

http://developers.popsical.com

`/dist` - swagger-ui fetches http://developers.popsical.com/api.json

## Developers

Edit api.yml to add/update endpoint specification.

## Steps to deploy

1. Edit `api.yml`. Use swagger 2.0 yaml syntax

2. Generate json `api.json` with `rake jsonify`. `bundle install` first if you can't run the rake

3. Upload `api.json` to s3 developers.popsical.com