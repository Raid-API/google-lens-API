# Google Lens Image Search API

Google Lens Image Search (Raid API)  –  find information about speeches around.

In this tutorial, we will show you how to use the Google Lens Image Search API from RapidAPI with Python, PHP, Ruby, and JavaScript examples. You will learn how to:

- Sign up for a RapidAPI account and subscribe to the Google Lens API
- Use the Google Lens API endpoints to get data
- Parse and display the data in your application

## Prerequisites

To follow this tutorial, you will need:

- A RapidAPI account. You can sign up for free here: [https://rapidapi.com/signup](https://rapidapi.com/auth/sign-up)
- A subscription to the Google Lens API. You can subscribe here: [Google Lens API](https://rapidapi.com/krmts-krmts-default/api/google-lens-image-search1)

## How to Use the Google Lens API

To use Google Lens API, you will need to provide two parameters:

- **x-rapidapi-key**: This is your RapidAPI key that authenticates your requests. You can find it in your RapidAPI dashboard.
- **x-rapidapi-host**: This is the host name of the API. For the Google Lens API, it is `google-lens-image-search1.p.rapidapi.com`.

### v1/google-lens/search/ 
#### Python example
```
import requests

url = "https://google-lens-image-search1.p.rapidapi.com/api/v1/google-lens/search/"

querystring = {"query_url":"YOUR-IMAGE-URL"}

headers = {
	"x-rapidapi-key": "SIGN-UP-FOR-KEY",
	"x-rapidapi-host": "google-lens-image-search1.p.rapidapi.com"
}

response = requests.get(url, headers=headers, params=querystring)

print(response.json())
```
### Example response
```json
{
  "Success": {
    "status": 200,
    "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
    "items": 60
  },
  "data": [
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://twitter.com/versenyjog",
      "image_url": "https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcQSBQa7xylxurvAugL6wdxwGsVSAokD7b8PIh-SxmdbeQY6CDGk",
      "title": "VJKK (@versenyjog) / X",
      "width": 386,
      "height": 130,
      "size": 4968
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://iabeurope.eu/knowledge_hub/privacy-by-design-exceeding-consumer-expectations-ipsos-and-google/",
      "image_url": "https://encrypted-tbn1.gstatic.com/images?q=tbn:ANd9GcTsniZgPnyWQsjjCtKnR9iZrug7UAWXuiDzmyYc-ReRl_YuPkjJ",
      "title": "Privacy by Design: Exceeding Customer Expectations - IPSOS and Google - IAB Europe",
      "width": 387,
      "height": 130,
      "size": 4963
    }
  ]
}
```

For list of endpoint and complete documentation, you can visit [Google Lens API](https://rapidapi.com/krmts-krmts-default/api/google-lens-image-search1)
