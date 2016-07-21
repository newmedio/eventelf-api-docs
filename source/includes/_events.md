# Events

## All Events

```shell
curl "http://www.eventelf.com/api/company/1/events" -H "Authorization: API_TOKEN"
```

> The above command would return the following JSON:

```json
{
  "events": [
    {
      "id": 1,
      "company_id": 1,
      "name": "Tulsa Run",
      "location_name": "Downtown Tulsa",
      "street_address": "6th & Boston Ave.",
      "city": "Tulsa",
      "state": "OK",
      "zipcode": "74120",
      "country": "US",
      "starts_on_date": "February 6, 2015",
      "ends_on_date": "February 8, 2015",
      "date_range": "February 6, 2015 - February 8, 2015",
      "currency": "USD",
      "currency_symbol": "$",
      "url": "http://eventelf.dev/events/1/login",
      "time_zone": "Central Time (US & Canada)",
      "created_at": "2014-09-18T12:01:24.516-05:00",
      "updated_at": "2014-11-12T10:42:31.196-06:00"
    },
    {
      "id": 2,
      "company_id": 1,
      "name": "Event Elf Run",
      "location_name": "Event Elf Headquarters",
      "street_address": "1234 S. Main St.",
      "city": "Tulsa",
      "state": "OK",
      "zipcode": "74120",
      "country": "US",
      "starts_on_date": "April 26, 2015",
      "ends_on_date": "April 26, 2015",
      "date_range": "April 26, 2015",
      "currency": "USD",
      "currency_symbol": "$",
      "url": "http://eventelf.dev/events/2/login",
      "time_zone": "Central Time (US & Canada)",
      "created_at": "2015-03-10T10:58:50.352-05:00",
      "updated_at": "2015-03-10T10:58:50.352-05:00"
    }
  ]
}
```

This endpoint retrieves all events for a given company.

### HTTP Request

`GET http://eventelf.com/api/company/COMPANY_ID/events`

## Upcoming Events

```shell
curl "http://www.eventelf.com/api/company/1/events/upcoming" -H "Authorization: API_TOKEN"
```

> The above command would return JSON identical to the 'All Events' endpoint

This endpoint retrieves all upcoming events for a given company.

### HTTP Request

`GET http://eventelf.com/api/company/COMPANY_ID/events/upcoming`

## Past Events

```shell
curl "http://www.eventelf.com/api/company/1/events/past" -H "Authorization: API_TOKEN"
```

> The above command would return JSON identical to the 'All Events' endpoint

This endpoint retrieves all past events for a given company.

### HTTP Request

`GET http://eventelf.com/api/company/COMPANY_ID/events/past`