# Amazon-price-tracker

> An app to keep track of amazon's products prices and to be notified when the value reaches a desired value via e-mail.

## Quick Start

``` bash
# Install dependencies for server
npm install dotenv nodemailer cheerio xmlhttprequest --save
```

``` bash
# Create a .env file with following variables with values storing gmail address and password from which mail needs to be sent
EMAIL_ADDRESS=""
PASSWORD=""
```

``` bash
# Run the application
node priceTracker.js <url_of_the_amazon_productpage_to_track> <min_price> <email_address_to_be_notified>
```

## Todos
 
 - [x] Build a scrapper
 - [x] Add Email Functionality
 - [ ] Add user login
 - [ ] Connect with MySQL Database
 - [ ] Deployable to Heroku

