# README

## Description

This application is built on `ruby 2.5.0` and `rails 5.2.3`

The core gem of this application is `shopify_app`. You can check it [here](https://github.com/Shopify/shopify_app)

If you want to know more what Shopify APIs provide, you can check it [here](https://help.shopify.com/en/api/reference/products/product#show)

## Quick Start

I assume that you have already registered as Shopify partner, created an application in your Shopify partner account and you had your own Shopify store. 

Just clone project and deploy it on your own `Heroku`

After that, please set environment variables for both your local and your Heroku environment

On local, you can create `.env` file and put in it content as below

```
api_key=YOUR_SHOPIFY_PARTNER_APP_API_KEY
api_secret=YOUR_SHOPIFY_PARTNER_APP_SECRET
```

Then, you can set those to your Heroku by just tying
```
heroku config:set api_key=YOUR_SHOPIFY_PARTNER_APP_API_KEY
heroku config:set api_secret=YOUR_SHOPIFY_PARTNER_APP_SECRET
```

Alternatively, you can download ngrok and start it using below command
```
./ngrok http 3000
```

## Gem Set


In this project, instead of using `ngrok`, I deploy it to heroku, u can check it [here](https://colin-shopify-custom-app.herokuapp.com/)

- `Httparty` gem to make call to Shopify API

- `RSPEC` as the testing framework 
- `FactoryBot` to create test data

- `Bootstrap 4` installed by gem `bootstrap`. You can check it [here](https://github.com/twbs/bootstrap-rubygem)
- `bootstrap_form` to create form with bootstrap

Project

## TESTING

In order to run the example test cases, you need to set up your shop domain & shop token first in your `.env` file

Then, you can simply run the command `rspec spec/requests`

