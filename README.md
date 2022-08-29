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

# Fampay Assignment

## Technologies Used

1. Frontend - ReactJs
2. Backend - NodeJs + ExpressJs
3. Database - MongoDB

## Quick Start
**Server Setup**

```bash
# Move to server folder and # Install dependencies
cd ../server
npm install

# Run the application
npm start
```

**Frontend Setup**

```bash
# Install dependencies by moving to frontend folder  
cd ../frontend
npm install

# Run the react application only
npm start
```

## Description

>> Server calls the YouTube API continuously in background with an interval of every `1 minute (60 seconds)` using `node-cron` package.

## Routes
- [GET] `/api/videos?perPage=__&page=__` - The endpoint returns stored video data in a paginated response sorted in descending order of published datetime. The response is as below
```json
{
    "status": "success",
    "data": {
        "videos": [
            {
                "_id": "630ce3ac43dcf3fe074e29b6",
                "videoId": "w22PQq_E58c",
                "title": "Which player do you like💯 #cricket #captain #short",
                "channelId": "UCi5lw2xfE3H_rGn8a5xQJ2w",
                "channelTitle": "GuDo bhai",
                "publishedAt": "2022-08-29T16:04:47.000Z",
                "description": "",
                "thumbnails": {
                    "default": {
                        "url": "https://i.ytimg.com/vi/w22PQq_E58c/default.jpg",
                        "width": 120,
                        "height": 90
                    },
                    "medium": {
                        "url": "https://i.ytimg.com/vi/w22PQq_E58c/mqdefault.jpg",
                        "width": 320,
                        "height": 180
                    },
                    "high": {
                        "url": "https://i.ytimg.com/vi/w22PQq_E58c/hqdefault.jpg",
                        "width": 480,
                        "height": 360
                    }
                },
                "__v": 0,
                "createdAt": "2022-08-29T16:05:00.873Z",
                "updatedAt": "2022-08-29T16:05:00.873Z"
            },
            {
                "_id": "630ce3ac43dcf3fe074e29b4",
                "videoId": "Kra-wdmAhrg",
                "title": "gk | cricket",
                "channelId": "UCCgiYhckOrJXqxe0_Sc146w",
                "channelTitle": "Gyaan galaxy AJIT",
                "publishedAt": "2022-08-29T16:04:17.000Z",
                "description": "",
                "thumbnails": {
                    "default": {
                        "url": "https://i.ytimg.com/vi/Kra-wdmAhrg/default.jpg",
                        "width": 120,
                        "height": 90
                    },
                    "medium": {
                        "url": "https://i.ytimg.com/vi/Kra-wdmAhrg/mqdefault.jpg",
                        "width": 320,
                        "height": 180
                    },
                    "high": {
                        "url": "https://i.ytimg.com/vi/Kra-wdmAhrg/hqdefault.jpg",
                        "width": 480,
                        "height": 360
                    }
                },
                "__v": 0,
                "createdAt": "2022-08-29T16:05:00.872Z",
                "updatedAt": "2022-08-29T16:05:00.872Z"
            },
            {
                "_id": "630ce3ac43dcf3fe074e29b5",
                "videoId": "Y6wCapCJ9cs",
                "title": "Last Moment || Win By Six Hardik Pandey #cricket #indianvspakistanmatch",
                "channelId": "UCjAfLdZJzmjnBsUJdKV1ofQ",
                "channelTitle": "Mr Unique Vlogs",
                "publishedAt": "2022-08-29T16:04:09.000Z",
                "description": "shorts #cricket #match #cricketheighlights #indian #pakistan #pakistanhaters #cricketnews #todaynews #hardikpandya #viratkohli ...",
                "thumbnails": {
                    "default": {
                        "url": "https://i.ytimg.com/vi/Y6wCapCJ9cs/default.jpg",
                        "width": 120,
                        "height": 90
                    },
                    "medium": {
                        "url": "https://i.ytimg.com/vi/Y6wCapCJ9cs/mqdefault.jpg",
                        "width": 320,
                        "height": 180
                    },
                    "high": {
                        "url": "https://i.ytimg.com/vi/Y6wCapCJ9cs/hqdefault.jpg",
                        "width": 480,
                        "height": 360
                    }
                },
                "__v": 0,
                "createdAt": "2022-08-29T16:05:00.872Z",
                "updatedAt": "2022-08-29T16:05:00.872Z"
            },
            {
                "_id": "630ce3ac43dcf3fe074e29b7",
                "videoId": "6MScftlMqBI",
                "title": "Ind vs Pak asia cup review🛐 / india successfully takes revenge🔥#shorts #cricket #indvspak #asiacup",
                "channelId": "UCsGQMzh0fP4zCnpsFe2M5Gw",
                "channelTitle": "PinkBall Edits",
                "publishedAt": "2022-08-29T16:04:06.000Z",
                "description": "",
                "thumbnails": {
                    "default": {
                        "url": "https://i.ytimg.com/vi/6MScftlMqBI/default.jpg",
                        "width": 120,
                        "height": 90
                    },
                    "medium": {
                        "url": "https://i.ytimg.com/vi/6MScftlMqBI/mqdefault.jpg",
                        "width": 320,
                        "height": 180
                    },
                    "high": {
                        "url": "https://i.ytimg.com/vi/6MScftlMqBI/hqdefault.jpg",
                        "width": 480,
                        "height": 360
                    }
                },
                "__v": 0,
                "createdAt": "2022-08-29T16:05:00.873Z",
                "updatedAt": "2022-08-29T16:05:00.873Z"
            }
        ],
        "pagination": {
            "totalCount": 22,
            "currentPage": 1,
            "perPage": 4
        }
    }
}
```

- [GET] `/api/search-videos?query_string=___` - The endpoint returns videos containing partial match for the search query in either video title or description.
