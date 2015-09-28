Categories
==========

Get Primary Categories
----------------------

 - `GET /api/category/primaries` will return all primary categories.
 
```json
[
  {
    "primary": "Cladding'",
    "primary_slug": "cladding"
  }
]
```

**Category Model Properties**

| Property | Description |
| -------- | ------------ |
| `primary` | Name of primary category.|
| `primary_slug` | Slugged name of primary category.|

*Use the `primary_slug` with the `primary` parameter when searching.*
 
 - `GET /api/search/?primary=cladding` where `cladding` is the `primary_slug` value.
 
See searching for products [here](search.md).
 


