# Company

## Single Company

```shell
curl "http://www.eventelf.com/api/companies/1" -H "Authorization: API_TOKEN"
```

> The above command would return the following JSON:

```json
{
  "id": 1,
  "name": "New Medio",
  "company_time_zone": "Central Time (US & Canada)",
  "support_email": "support@newmediotesting.com",
  "support_phone": "9184441234",
  "notification_email": "notifications@newmediotesting.com"
}
```

This endpoint retrieves the details for a given company.

### HTTP Request

`GET http://eventelf.com/api/companies/COMPANY_ID`