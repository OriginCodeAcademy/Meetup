# Chipotle Mapper

## Description
![Chipotle Muh Life](http://media.giphy.com/media/phGm2TPqh25EY/giphy.gif)

Everybody loves Chipotle. We're going to build a small web app that shows you where your nearest Chipotle is.

## Scope
* The app will show the closest Chipotle restaurants based on the users current location.
* The app will not accept orders - this is a limitation of the API.

## Requirements
* The web app must get the users location from the browser.
* The web app must make use of the Chipotle API provided by Origin. 

## High Level Tasks
* [ ] Create a GitHub repository called ChipotleMapper on your account
* [ ] Build the app on your local machine
* [ ] Commit the app and push to GitHub

## Helpful Hints
* [Checkout the Google Maps Javascript library](https://developers.google.com/maps/documentation/javascript/examples/) to see how to integrate Google Maps into your project
* Research the Chipotle API below
* You can use the [$.getJSON](http://api.jquery.com/jquery.getjson/) method in jQuery to call our Chipotle API 
* Find a JSON extension for your browser so you can checkout the raw data returned by the API (Example, [here's one for Chrome](https://chrome.google.com/webstore/detail/json-formatter/bcjindcccaagfpapjjmafapmmgkkhgoa?hl=en))

## Learning Goals
By the end of this project, you'll have learned:

* How to read documentation to integrate third party libraries into your project
* How to research an API to make use of it in your app
* How to use results of an API to provide additional functionality to your apps
* That Chipotle is now yur laif.

## Chipotle API
Here's a description of our API - You can visit this API in your browser to see the raw data that gets returned.

### URL
```
http://linux.cwserve.com:24785
```

### Endpoints
**Restaurants**
```
/restaurants/<zip_code>
```

Example Request
```
http://linux.cwserve.com:24785/restaurants/92101
```

Example Response
```json
[
	{
		"id": 1635,
		"name": "101 West Broadway",
		"address": {
			"formattedAddress": "101 West Broadway, San Diego, CA 92101, USA",
			"latitude": 32.7148692,
			"longitude": -117.1640955,
			"extra": {
				"googlePlaceId": "ChIJxVasOqhU2YARvXy9Ybjj5xk",
				"confidence": 1,
				"premise": null,
				"subpremise": null,
				"neighborhood": "Downtown",
				"establishment": null
			},
			"administrativeLevels": {
				"level2long": "San Diego County",
				"level2short": "San Diego County",
				"level1long": "California",
				"level1short": "CA"
			},
			"streetNumber": "101",
			"streetName": "West Broadway",
			"city": "San Diego",
			"country": "United States",
			"countryCode": "US",
			"zipcode": "92101"
		}
	}
]
```
