Find Products
==========

Search for products
----------------------

 - `GET /api/search` will return all products.
 
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




| Parameter     | Required | Example                                                                                                                          |
| ------------- | -------- | -------------------------------------------------------------------------------------------------------------------------------- |
| `search: string` | false    | `GET /api/search?search=chair` will get all products found containing chair(s).  |
| `company: string` | false    | `GET /api/search?company=lundia` will get all products by company.  |
| `primary: string` | false    | `GET /api/search?primary=chair` will get all products found for the primary category provided.  |
| `secondary: string` | false    | `GET /api/search?primary=&secondary=` will get all products found for the primary and secondary categories provided.  
when using the secondary category the primary category must be included|
| `tertiary: string` | false    | `GET /api/search?search=chair` will get all products found for the primary, secondary, and tertiary categories provided.  |
| `page: string` | false    | `GET /api/search?search=chair` will get all products found containing chair(s).  |