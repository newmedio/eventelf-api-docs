# Events

## All Events

```shell
curl "http://www.eventelf.com/api/companies/1/events" -H "Authorization: API_TOKEN"
```

> The above command would return the following JSON:

```json
{
	"events": [
		{
			"id": 1,
			"company_id": 1,
			"name": "New Medio Run",
			"active": true,
			"location_name": "New Medio",
			"street_address": "233 S. Detroit Ave., Ste 202",
			"city": "Tulsa",
			"state_abb": "OK",
			"state": "Oklahoma",
			"zipcode": "74120",
			"country": "US",
			"formatted_address": "233 S. Detroit Ave., Ste 202, Tulsa, OK, 74120",
			"starts_on_date": "February 6, 2015",
			"ends_on_date": "February 8, 2015",
			"date_range": "February 6, 2015 - February 8, 2015",
			"currency": "USD",
			"currency_symbol": "$",
			"url": "http://eventelf.dev/events/1/login",
			"sponsor_image_url": null,
			"time_zone": "Central Time (US & Canada)",
			"created_at": "2014-09-18T12:01:24.516-05:00",
			"updated_at": "2014-11-12T10:42:31.196-06:00"
		},
		{
			"id": 2,
			"company_id": 1,
			"name": "Event Elf Fun Run",
			"active": true,
			"location_name": "Event Elf Headquarters",
			"street_address": "1234 S. Main St.",
			"city": "Tulsa",
			"state_abb": "OK",
			"state": "Oklahoma",
			"zipcode": "74120",
			"country": "US",
			"formatted_address": "1234 S. Main St., Tulsa, OK, 74120",
			"starts_on_date": "April 26, 2015",
			"ends_on_date": "April 26, 2015",
			"date_range": "April 26, 2015",
			"currency": "USD",
			"currency_symbol": "$",
			"url": "http://eventelf.dev/events/2/login",
			"sponsor_image_url": "https://d1mapbwzxiat0v.cloudfront.net/attachments/5459cfa9338e3560290cc22a29f252dd33a8e180/store/482d64cd2d71b7c71c8ee601bdd9e76ca840aacd04a5ef2b4fd2f733e50b/logo.jpg",
			"time_zone": "Central Time (US & Canada)",
			"created_at": "2015-03-10T10:58:50.352-05:00",
			"updated_at": "2015-03-10T10:58:50.352-05:00"
		}
	]
}
```

This endpoint retrieves all events for a given company.

### HTTP Request

`GET http://eventelf.com/api/companies/COMPANY_ID/events`

## Upcoming Events

```shell
curl "http://www.eventelf.com/api/companies/1/events/upcoming" -H "Authorization: API_TOKEN"
```

> The above command would return JSON identical in structure to the 'All Events' endpoint

This endpoint retrieves all upcoming events for a given company.

### HTTP Request

`GET http://eventelf.com/api/companies/COMPANY_ID/events/upcoming`

## Past Events

```shell
curl "http://www.eventelf.com/api/companies/1/events/past" -H "Authorization: API_TOKEN"
```

> The above command would return JSON identical in structure to the 'All Events' endpoint

This endpoint retrieves all past events for a given company.

### HTTP Request

`GET http://eventelf.com/api/companies/COMPANY_ID/events/past`

## Single Event

```shell
curl "http://www.eventelf.com/api/companies/1/events/231" -H "Authorization: API_TOKEN"
```

> The above command would return the following JSON:

```
{
	"id": 94,
	"name": "Toddlers Ticketing Event 2015",
	"description": "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas nec eleifend purus, eu luctus leo. Fusce dapibus tincidunt est, quis bibendum erat consequat ac. Nam laoreet velit eget felis venenatis mollis. Suspendisse potenti. Ut eu ultrices dui.",
	"restrictions": "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas nec eleifend purus, eu luctus leo. Fusce dapibus tincidunt est, quis bibendum erat consequat ac. Nam laoreet velit eget felis venenatis mollis. Suspendisse potenti. Ut eu ultrices dui.",
	"disclaimer": "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas nec eleifend purus, eu luctus leo. Fusce dapibus tincidunt est, quis bibendum erat consequat ac. Nam laoreet velit eget felis venenatis mollis. Suspendisse potenti. Ut eu ultrices dui.",
	"active": true,
	"divisions": [
		{
			"id": 95,
			"name": "Day 1",
			"starts_on": "2025-12-16",
			"active": true,
			"registration_activities": [],
			"ticketed_activities": [
				{
					"id": 25,
					"name": "Private Shindig",
					"description": "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas fermentum in nulla quis tincidunt. Donec dictum egestas dapibus. Duis sit amet leo lectus. Phasellus cursus erat id turpis hendrerit, et ultrices nibh consectetur.",
					"expires_at": "2020-12-31T17:30:00.000-06:00",
					"total_spots": 200,
					"num_spots_purchased": 3,
					"num_spots_left": 197,
					"spots_remaining_threshold": 100,
					"active": true,
					"all_access": false,
					"private": true,
					"price": "54.0",
					"dated_prices": [
						{
							"id": 10,
							"price": "20.0",
							"valid_until": "2016-06-22T23:59:00.000-05:00"
						}
					]
				},
				{
					"id": 24,
					"name": "Wave 1",
					"description": "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas nec eleifend purus, eu luctus leo. Fusce dapibus tincidunt est, quis bibendum erat consequat ac. Nam laoreet velit eget felis venenatis mollis. Suspendisse potenti. Ut eu ultrices dui.",
					"expires_at": "2025-12-16T17:00:00.000-06:00",
					"total_spots": 200,
					"num_spots_purchased": 6,
					"num_spots_left": 194,
					"spots_remaining_threshold": 100,
					"active": true,
					"all_access": false,
					"private": false,
					"price": "25.0",
					"dated_prices": [
						{
							"id": 11,
							"price": "50.0",
							"valid_until": "2016-05-18T23:59:00.000-05:00"
						},
						{
							"id": 9,
							"price": "20.0",
							"valid_until": "2016-06-21T23:59:00.000-05:00"
						}
					]
				}
			]
		}
	]
}
```

This endpoint retrieves the details of a given event including ticketed and non-ticketed activity information. If any activities have dated pricing information, it will be returned also.

### HTTP Request

`GET http://eventelf.com/api/companies/COMPANY_ID/events/EVENT_ID`