Find Products
==========

Search for products
----------------------

 - `GET /api/search` will return all products.
 


| Parameter     | Required | Example                                                                                                                          |
| ------------- | -------- | -------------------------------------------------------------------------------------------------------------------------------- |
| `search: string` | false    | `GET /api/search?search=chair` will get all products found containing chair(s).  |
| `company: string` | false    | `GET /api/search?company=lundia` will get all products by the company 'Lundia.'  |
| `primary: string` | false    | `GET /api/search?primary=cladding` gets all products found for the primary category 'cladding.'  |
| `secondary: string` | false    | `GET /api/search?primary=cladding&secondary=weatherboards` gets all products found for the primary category 'cladding' and secondary category 'weatherboards.' <br> When using the secondary category the primary category must be included.|
| `tertiary: string` | false    | `GET /api/search?primary=cladding&secondary=weatherboards&tertiary=pvc-weatherboards` will get all products found for the primary, secondary, and tertiary categories provided.  |
| `page: string` | false    | `GET /api/search?page=2` returns the results for page number '2.'  |

**Compound Filters**

*Any and all of the query strings parameters my be combined to better filter results*


| Compound Query | Example |
| ------ | ------- |
| `GET /api/search?search=chair&company=lundia` | Returns products that match the 'chair' search query and belong to the company 'Lundia.' |
| `GET /api/search?page=3&company=steel-and-tube&primary=cladding` | Returns products that belong to the 'cladding' primary category, belong to the company 'Steel & Tube' and is 3 pages deep in the result set.  |

**Filter Model**

```json
{
    "filters": [
        {
            "filter_items": [
                {
                    "count": 6,
                    "slug_value": "lundia",
                    "value": "Lundia"
                },
                {
                    "count": 1,
                    "slug_value": "polyflor",
                    "value": "Polyflor"
                }
            ],
            "filter_key": "companies"
        },
        {
            "filter_items": [
                {
                    "count": 1,
                    "slug_value": "adhesives-and-compounds",
                    "value": "Adhesives & Compounds"
                },
                {
                    "count": 1,
                    "slug_value": "exterior-and-landscape",
                    "value": "Exterior & Landscape"
                }
            ],
            "filter_key": "primary_categories"
        }
    ],
    "products": [
        {
            "company_name": "Lundia",
            "company_slug": "lundia",
            "image": "https://ps-content.s3.amazonaws.com/product/4da61cd84ff399d11457cb90/images/4da61cfd4ff39ad1cc056068/1033-md.jpg",
            "product_id": "4da61cd84ff399d11457cb90",
            "product_slug": "uni-chair",
            "product_title": "Uni Chair"
        },
        {
            "company_name": "Poynters",
            "company_slug": "poynters",
            "image": "https://ps-content.s3.amazonaws.com/product/4db645334ff399d11457cbf4/images/4db645464ff39ad1cc0560df/7_1-md.jpg",
            "product_id": "4db645334ff399d11457cbf4",
            "product_slug": "espresso-chair",
            "product_title": "Espresso  chair"
        }
    ],
    "total": 75
}
```

| Property | Description |
| -------- | ------------ |
| `total: number` | Total number of products found for the query (25 results returned per request).|
| `products: array of products` | Products found matching the query. |
| `filters: array` | The filters array contains all filters that match the query provided.  Use the `slug_value` and `filter_key` to build query.|

**Status Codes**
- `200 OK` will be returned if query is successful.
- `404 Not Found` will be returned if URL is poorly formed.

See getting a single product [here](product.md).


