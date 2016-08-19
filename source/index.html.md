---
title: Event Elf API Documentation

language_tabs:
  - shell

toc_footers:
  - <a href='http://www.eventelf.com/sign_up'>Sign Up for an Event Elf Account</a>
  - <a href='https://github.com/lord/slate'>Documentation Powered by Slate</a>

includes:
  - company
  - events

search: true
---

# Introduction

Welcome to the Event Elf API. You can use this API to access your event data after you have [signed up](http://www.eventelf.com/sign_up) as a company on the Event Elf platform.

Once you have successfully created an account, the API Token needed to make authenticated requests can be found in company settings. [Login here](http://www.eventelf.com/admin) with your administrator credentials.

# Authentication

```shell
# With shell, you can just pass the correct header with each request
curl "http://www.eventelf.com/api/API_ENDPOINT" -H "Authorization: Token token=API_TOKEN"
```

Event Elf uses API keys to allow access to the API. You can access your API token in the [administration area](http://www.eventelf.com/admin).

Event Elf expects for the API token to be included in all API requests to the server in a header that looks like the following:

`Authorization: Token token=API_TOKEN`

<aside class="notice">
You must replace <code>API_TOKEN</code> with your company's API token.
</aside>