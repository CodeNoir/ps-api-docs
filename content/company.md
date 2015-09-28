Categories
==========

Get Companies
----------------------

 - `GET /api/company/all` will return all companies that are available for your api_key.
 
```json
[
  {
    "_id": "471fce454ff399d11457bc0c",
    "name": "Fairview Systems",
    "slug": "fairview-systems"
  }
]
```

**Company Model Properties**

| Property | Type | Description |
| -------- | ---- | ----------- |
| `_id` | string | comapny identifier |
| `name` | string | Name of company.|
| `slug` | string | Slugged name of company.|

*Use the `slug` with the `company` parameter when searching.*
 
 - `GET /api/search/?company=fairview-systems` where `fairview-systems` is the `slug` value.
 
See searching for products [here](search.md).
 
