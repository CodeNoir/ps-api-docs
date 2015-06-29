Categories
==========

Get Primary Categories
----------------------

 - `GET /api/category/primaries` will return all primary categories.
 
```json
[
  {
    "primary": "Cladding'",
    "primary_slug": 47
  }
]
```

**Category Model Properties**

| Property | Description |
| -------- | ------------ |
| `primary` | name of primary category|
| `primary_slug` | slugged name of primary category|

*Use the `primary_slug` with the `primary` parameter when searching*
 
 - `/search/primary=cladding` where `cladding` is the `primary_slug` value
 
See searching for products [here](search.md)
 


