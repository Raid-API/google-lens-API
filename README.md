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
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.linkedin.com/posts/dmlaorg_idmlc-digitalmedialicensing-googlesponsor-activity-7113161991342493696-3dPX?trk=public_profile_like_view",
      "image_url": "https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcRYrtI1TdnvyCpMP5KAMzUW3Uf9QV-hLHHsA6M45ZJXtyKNQ62A",
      "title": "Digital Media Licensing Association - DMLA on LinkedIn: #idmlc #digitalmedialicensing #googlesponsor #content #copyright…",
      "width": 394,
      "height": 128,
      "size": 9869
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.wgvunews.org/the-wgvu-morning-show/2023-03-31/google",
      "image_url": "https://encrypted-tbn1.gstatic.com/images?q=tbn:ANd9GcREOcD57wipdZLY8RkjQuAPd018fo4CYEg8XH0MFWQwPdzyfJ00",
      "title": "Google | WGVU NEWS",
      "width": 386,
      "height": 130,
      "size": 9594
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://device.report/manual/2876420",
      "image_url": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcScjNp92rNv98FJvYfKzDIVlhpKkhnZfY_H4ZSyirky84UlhDPv",
      "title": "Google GA02411-US Nest Cam with Floodlight - Snow User Manual",
      "width": 386,
      "height": 130,
      "size": 7291
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.linkedin.com/posts/avinash-singh-071b79175_hiring-jobs-jobseekers-activity-7116705434123587584-SZ-s",
      "image_url": "https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcSipsV0yvXFzLUn4wGywJeiJ4tEIN6SgM9QzHHhG3iHoGEX2wCG",
      "title": "Avinash Singh on LinkedIn: #hiring #jobs #jobseekers #internship #intern #freshers #hiringalert",
      "width": 386,
      "height": 130,
      "size": 9682
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.ajournalofmusicalthings.com/googles-list-of-the-most-search-songs-of-2022-will-surprise-you/",
      "image_url": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTk6Dhkxw_R6bSCyRRWLD764Ramw-jeuCYmTtaEHo-CGdYH3Qvq",
      "title": "Google's list of the most-searched songs of 2022 will surprise you",
      "width": 386,
      "height": 130,
      "size": 7379
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.linkedin.com/posts/jane-sadler-65896b100_member-spotlight-google-activity-6845423675186012160-vGUU",
      "image_url": "https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcQgpYJDQP_Y5uiUd2zytGwIsjRQAVFI-6_iKxTfUhIjeqnyEs91",
      "title": "Jane Sadler on LinkedIn: Member Spotlight: Google",
      "width": 386,
      "height": 130,
      "size": 9153
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://uk.linkedin.com/in/michael-pugh-47814452",
      "image_url": "https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcQvuvqrwwqM47UuM16NFCTbTbBmJlBOI94YCoTnTMyu1oyKJy7u",
      "title": "Michael Pugh | LinkedIn",
      "width": 380,
      "height": 133,
      "size": 8293
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.quora.com/What-are-the-requirements-to-become-a-project-manager-at-Google-Facebook-or-Amazon",
      "image_url": "https://encrypted-tbn1.gstatic.com/images?q=tbn:ANd9GcQOZmYpcUBlMnHTcCbqYFAInLkxxrNPmb4ZOiA5omanNJ_TFaKl",
      "title": "What are the requirements to become a project manager at Google, Facebook or Amazon? - Quora",
      "width": 386,
      "height": 130,
      "size": 5303
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://weareon.org/index.php/who-we-are/",
      "image_url": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcScdX1B9vmTTviqwe1BnoFdnLlKebLzpwPjIOFDTMcXzvuZJx2j",
      "title": "Who We Are - WeAreOn",
      "width": 386,
      "height": 130,
      "size": 5029
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.tewkesburymotorsales.com/testimonials/",
      "image_url": "https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcRXUIDGkQKUqcMnnN58U35Bg90WfJI_eZxGxv5RvB0RfAh73AeF",
      "title": "Testimonials - Tewkesbury Motor Sales",
      "width": 386,
      "height": 130,
      "size": 4761
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.linkedin.com/pulse/has-google-just-killed-cold-calling-daniel-disney",
      "image_url": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR-0uRTbqeHjrJr739RMarq5bprURiCTaK28C-H14eLA4lFrjVp",
      "title": "Has Google Just Killed Cold Calling?",
      "width": 386,
      "height": 130,
      "size": 4914
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.facebook.com/HRflowSoftware/",
      "image_url": "https://encrypted-tbn1.gstatic.com/images?q=tbn:ANd9GcSNmhq29knaUdJEJVz48TweyL4frR6BUcVLpcLK8tXVT2O3lSJO",
      "title": "HR Flow | Edinburgh",
      "width": 386,
      "height": 130,
      "size": 4914
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://annarborusa.org/news/businesses/google/",
      "image_url": "https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcQqo7Zyc6IlDbpU39gLIoDLXnreEHGpuj8FSe38LkYQpTRRBuhq",
      "title": "Google - Ann Arbor SPARK",
      "width": 386,
      "height": 130,
      "size": 5035
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://easysitehire.com.au/reviews/",
      "image_url": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRqsaGMN2kuSHSxcFe1PklshdmKKgzys_a3MgGvEnp2SEErwTVj",
      "title": "Trusted Reviews and Testimonials for Easy Site Hire",
      "width": 387,
      "height": 130,
      "size": 9042
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.marinsoftware.com/industries/retail",
      "image_url": "https://encrypted-tbn1.gstatic.com/images?q=tbn:ANd9GcQhqh3J_Cib8musaQofQ_wvGEbKwecn2340baqHz4FqciuwOagW",
      "title": "Retail Advertising Solution",
      "width": 386,
      "height": 130,
      "size": 4978
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://weareevolved.com/online-hotel-booking-software/",
      "image_url": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS6fK3fXycN6TIQMeQnR7YBSEwAVrANvvKIjVPTibFcGqunbtmv",
      "title": "Online Hotel Booking Software - EVOLVED Agency",
      "width": 387,
      "height": 130,
      "size": 5278
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://broadly.com/blog/how-to-grow-small-business/",
      "image_url": "https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcTNsHZtG5O0ZIaLFu88plpaYfXnK1acV1VDWEySKebjc1Z7Nkxk",
      "title": "51 Marketing Ideas To Grow Your Small Business in 2023 - Broadly.com",
      "width": 387,
      "height": 130,
      "size": 5136
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.trivillageselfstorage.com/resources/tri-village-self-storage-reviews/",
      "image_url": "https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcQX4WBZB-eK2f39v8uoQu4zlIiM8BfHf92IgT7d8CFmJA4Fk6Mj",
      "title": "Tri-Village Self Storage Reviews - Tri-Village Self Storage",
      "width": 379,
      "height": 133,
      "size": 6062
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://switchonmymedia.com/technology-business-solutions/",
      "image_url": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRtVAWQWGxJ4TLTpfDXmhSrK3X-8em7O4SpVrft6xraef0heGOB",
      "title": "Technology   Business Solutions - SwitchonMyMedia.com",
      "width": 387,
      "height": 130,
      "size": 9985
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://sharpspring.com/ads/get-a-demo/",
      "image_url": "https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcQBJunC6v8z1dokDCmdlzFbWYOpwsuXBfYhJMxmKqOxU8y-MAN8",
      "title": "Schedule a live, personal demo today | SharpSpring Ads",
      "width": 387,
      "height": 130,
      "size": 4829
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.searchengineneed.com/webtools/google-serp-preview-tool/",
      "image_url": "https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcQbFwIyE626wNoU4ehFhV5RWQeZ6d_nTvGTJBogDyARL7E3eYOB",
      "title": "Google SERP Snippet Preview Tool - Free & User-friendly",
      "width": 387,
      "height": 130,
      "size": 9512
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.sully.ai/",
      "image_url": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRjcNNI1ltxhUWjEP-wfvs_eMjmrWAtK2MhbBl5G_3l36tHmZhW",
      "title": "Sully.ai - AI team to automate healthcare tasks",
      "width": 390,
      "height": 129,
      "size": 5834
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.felicecurcelli.net/portfolio.html",
      "image_url": "https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcQuarhwH0-K8qR93tIFodmsMLfV6Do7SMtKZivRJigLr0LPLCcH",
      "title": "Felice Curcelli, Portfolio - FELICE CURCELLI",
      "width": 386,
      "height": 130,
      "size": 5301
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "http://roryjmurphy.com/about-rory.html",
      "image_url": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR1-nmfVzCzkqJNhCYAeP-jibilST2imtu-exLJR3shshDxncfc",
      "title": "ABOUT RORY | roryjmurphy.com",
      "width": 404,
      "height": 125,
      "size": 5135
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.renewableinstitute.org/testimonials/",
      "image_url": "https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcRByc6tS2iE5WT0_zyUhDonHEIqzo_CXIYSTVzq3AYrjQwGsIKB",
      "title": "Testimonials - The Renewable Energy Institute",
      "width": 389,
      "height": 129,
      "size": 7215
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://community.withairbnb.com/t5/Help/Guests-want-to-check-in-at-1-a-m/td-p/134128",
      "image_url": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQquIN4-_SdNqAIrnXaUez8vzlGWyn23ZbKU8ROW7zWsu55j9Tx",
      "title": "Solved: Guests want to check in at 1 a.m. - Airbnb Community",
      "width": 386,
      "height": 130,
      "size": 5301
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://purestay.co.uk/letting-agents/",
      "image_url": "https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcRFHBFDtZuxI26KW-irXuCQUg9xLbuNqGDbc8d_JF3zMAocQgKv",
      "title": "Letting Agents - PureStay",
      "width": 386,
      "height": 130,
      "size": 5252
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://betterstudio.com/fonts/google-logo-font/",
      "image_url": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRef5C7YQ8lU9x5iPLbTKw0-SL4uLl4Foj3dR2RzhPMAgNyYUHo",
      "title": "Google Logo Font: Download Free Font & Logo",
      "width": 386,
      "height": 130,
      "size": 9744
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.linkedin.com/pulse/google-adwords-certifications-spencer-paullin",
      "image_url": "https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcRKn2aSW-5dVYVasKrcjQDrZXaT76RVf9Guf70a7CaMgiqW7xoe",
      "title": "Google AdWords Certifications",
      "width": 386,
      "height": 130,
      "size": 6583
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.thesun.ie/tech/news-tech/10266077/google-logo-colors-change/",
      "image_url": "https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcRBAzsbZuNz9raPmULkrAEneyp-K-W8qFXCD2vPIgUanEtDpTUJ",
      "title": "People are just realizing the Google logo has changed its colors five times – including sneaky 2015 switch | The Irish Sun",
      "width": 387,
      "height": 130,
      "size": 9151
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://twitter.com/awordaboutwind",
      "image_url": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSzQs4-Tr-a5hrh92N91N4yAqE2LNLdjTXTVXWIuy-oZW2YFw6U",
      "title": "A Word About Wind (@awordaboutwind) / X",
      "width": 387,
      "height": 130,
      "size": 9706
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.pinterest.com/pin/859132066392631120/",
      "image_url": "https://encrypted-tbn1.gstatic.com/images?q=tbn:ANd9GcTIUsASwcLqtaoIGeGJPFYqnQLeLfcla4pJVYJFwCh5p3-C8Oho",
      "title": "Google Logo 2015 PNG Image | Google logo, Search engine optimization, Social media",
      "width": 386,
      "height": 130,
      "size": 9403
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.robertocarlosfitness.com/personal-training-testimonials/",
      "image_url": "https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcSnRLGbsAA_5O24pTZbl68nyYyB18AbosFh6t-3NAiYF-jIZJHf",
      "title": "Lift:RCFitness Gym Fitness Testimonials | See what our clients have to say",
      "width": 387,
      "height": 130,
      "size": 4970
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://qubed.ro/10-motive-pentr-a-va-simplifica-logo/",
      "image_url": "https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcRIQzCWnF7Ml4jgcMpL-_mGPE2_2iFevc9KteSVwjkwuwbH_0t3",
      "title": "10 motive pentru a vă simplifica logo - Qubed Agency | Agenție de branding și web design",
      "width": 386,
      "height": 130,
      "size": 7038
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://shinkalion.fandom.com/wiki/Google",
      "image_url": "https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcTKGF1AcnR2QcgSIOW-4-9mnggnehbVQBL9W-MPUzRHzQpdEP54",
      "title": "Google | Shinkalion Wiki | Fandom",
      "width": 386,
      "height": 130,
      "size": 4928
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://calmcode.io/testimonials.html",
      "image_url": "https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcSS8jqEo0StLCweTCEU23LSiPT0hzLx_v2K9qgrDgGfMm5Pb-X5",
      "title": "calmcode - learn code calmly",
      "width": 368,
      "height": 124,
      "size": 4076
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://uspto.report/TM/85531517",
      "image_url": "https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcS4l9OVZe3Hsnd4XQThjrIcV4bS5bvtn6TWD36oy2EyKiTDWJcY",
      "title": "GOOGLE - Google Llc Trademark Registration",
      "width": 386,
      "height": 130,
      "size": 9665
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.adsbyjohn.com/google-vibe",
      "image_url": "https://encrypted-tbn1.gstatic.com/images?q=tbn:ANd9GcQEZECuAz7jsbvVk72JCBY7_ZFuvmNTQA5c0ABtgAGEWhnlZPnq",
      "title": "Ads By John - Google Vibe",
      "width": 374,
      "height": 122,
      "size": 5935
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://twitter.com/camitechdesign",
      "image_url": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQeL2Uov__KI143VSXQhPQK0aU_Mr4sZ-uPDzGWvHTe434LiCgG",
      "title": "Cami Tech Design (@camitechdesign) / X",
      "width": 387,
      "height": 130,
      "size": 7888
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.aceolution.com.au/",
      "image_url": "https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcQS49QdBZW3qav7_EsgA64PudnTITWXNQBnrVOpBy2J0XVdtgln",
      "title": "aceolution – aceolution- IT services | Media solution",
      "width": 387,
      "height": 130,
      "size": 5307
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.madebytribe.com/who-we-are/",
      "image_url": "https://encrypted-tbn1.gstatic.com/images?q=tbn:ANd9GcR35Pa85v7DIT2zCPic7TYwPPSgc_vWIGTKIHd2mZL3H3YQuOUU",
      "title": "Who We Are - Tribe Interactive",
      "width": 387,
      "height": 130,
      "size": 5080
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://medium.com/@thejigsaw.in/top-search-engines-of-2018-b841f0faef8f",
      "image_url": "https://encrypted-tbn1.gstatic.com/images?q=tbn:ANd9GcRzrGIfQaCIB9DPIpHeb5AsdiuplekuqZHmHWCs_W4fZduWNY7o",
      "title": "Top Search Engines of 2018. You may know that the search engines… | by Shashank Sharma | Medium",
      "width": 387,
      "height": 130,
      "size": 5014
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://uk.linkedin.com/in/lee-hussain-a7014151",
      "image_url": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQirkPxZG7Iij2wM63WOl8UEqxQ9_Qijcx1lD8xesd3m3tOHplu",
      "title": "lee hussain - Managing Director - ENVIRO CITY | LinkedIn",
      "width": 386,
      "height": 130,
      "size": 9251
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://ca.linkedin.com/in/sijia-ding-860b75206",
      "image_url": "https://encrypted-tbn1.gstatic.com/images?q=tbn:ANd9GcTL8uH6xbuDOsGJ1mOwoA4a_vdPcu9Iyv2N334B7Oun5hk_jm5h",
      "title": "Sijia Ding - Software Developer - Google | LinkedIn",
      "width": 394,
      "height": 128,
      "size": 9430
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.blue.ai/",
      "image_url": "https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcQ6xltN28vP5H0R0V_gTY8qrigVv8wbIhXiHn0yaAw9SuHXkfUn",
      "title": "Home | Blue.Ai",
      "width": 386,
      "height": 130,
      "size": 5215
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.facebook.com/TTTElectric/",
      "image_url": "https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcR-6wrOkZjDdSma9SNeWivL3_VY2eRUVy9vca_ruv52zBuyKaew",
      "title": "Triple T Electric",
      "width": 386,
      "height": 130,
      "size": 9022
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://epistem.ie/wp-content/uploads/2022/03/Numeracy-Meet-2.pdf",
      "image_url": "https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcTYSchMYhQGIi0oW0Zuj9iA1elkWWgdC-Z04hwnaCJD4XI4u7fj",
      "title": "Title — Calibri Bold 26pt",
      "width": 387,
      "height": 130,
      "size": 4564
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.reddit.com/r/thehatedone/comments/cfgktb/alternatives_to_google_products_and_services/",
      "image_url": "https://encrypted-tbn1.gstatic.com/images?q=tbn:ANd9GcRPyA5HQ8wl4_TIqiD_ChecQUdJZaI61QcXcBaD5ZdXVwXlZ03z",
      "title": "Alternatives to Google products and services : r/thehatedone",
      "width": 386,
      "height": 130,
      "size": 9603
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://gems.engie.com/global-presence/germany/",
      "image_url": "https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcQctKn3HDIzGYKZdHZi68asOK7hV5_dUTfrho71KCPxcUo7B31y",
      "title": "Germany | ENGIE Global Energy Management & Sales",
      "width": 387,
      "height": 130,
      "size": 5070
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://thenationonlineng.net/googles-2020-year-in-search/",
      "image_url": "https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcQxQe2FoTk2WFPlaUIUplsCspjDZemXhUIJSc_XB570NGJJwt3Q",
      "title": "Google’s 2020 year in search | The Nation",
      "width": 294,
      "height": 171,
      "size": 5970
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.linkedin.com/in/liza-bukingolts",
      "image_url": "https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcR7lEsYH6mlYwoSoiMS0Uhv9lCvva7wanAv0bldjS-8ytMbb4Fa",
      "title": "Liza Bukingolts | LinkedIn",
      "width": 390,
      "height": 129,
      "size": 10096
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://winthe.cloud/",
      "image_url": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRo9mqSk8bvK3Ypty6_n2Sd5h24aJwDsUsziAh-sN3iHuDm2B8i",
      "title": "Win The Cloud - Become a 🚀 Cloud Solution Architect",
      "width": 387,
      "height": 130,
      "size": 6392
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.leadworx.com/",
      "image_url": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTMs0bD4YrdEKdzTsH_3y7FkXojL-kWeYslgu0sXM-JDhFXZ_gk",
      "title": "Home - Leadworx - Lead flashing supplies",
      "width": 387,
      "height": 130,
      "size": 6482
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.ssw.com.au/rules/rules-to-better-google-rankings-and-seo/",
      "image_url": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSwHIXaqWPgJVo0fcC94rYTsqyG52PtxjpmNtKX2KlfKOXkaQGu",
      "title": "SSW.Rules | Rules to Better Google Rankings and SEO",
      "width": 386,
      "height": 130,
      "size": 5477
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://madisoninnmv.com/reviews/",
      "image_url": "https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcQBlqFsYYKD6eUsaaC4LsDRkbKQPHTuUIaA7H4-0Rk24mkm4JZA",
      "title": "Best Places to Stay on Martha's Vineyard - Reviews | Madison Inn Oak Bluffs Hotel",
      "width": 387,
      "height": 130,
      "size": 7900
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.appgeo.com/what-we-do/",
      "image_url": "https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcTK9MqoT9NE_sg9_yAQ5XeSoWqBoU2Z6DLFj24c9QwcWpAPF-rP",
      "title": "Professional GIS Consulting Services - AppGeo",
      "width": 387,
      "height": 130,
      "size": 4759
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://www.linkedin.com/in/sriram-vemparala-77845737",
      "image_url": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ9iHS-VQkSsND5CfScTODlR3AUTN3esku4i7_otvB4WcKNzfYS",
      "title": "Sriram Vemparala | LinkedIn",
      "width": 392,
      "height": 129,
      "size": 9576
    },
    {
      "query_url": "https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png",
      "platform": "google lens",
      "page_url": "https://digitalskills21.com/en/accreditation-2/",
      "image_url": "https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcTbPA79mETK5z7NDu7b6W32Sw8HfyjXRayKzeX5udJKQWZs8h3D",
      "title": "Accreditation - Digital Skills21 Institution",
      "width": 387,
      "height": 130,
      "size": 4999
    }
  ]
}
```

For list of endpoint and complete documentation, you can visit [Google Lens API](https://rapidapi.com/krmts-krmts-default/api/google-lens-image-search1)