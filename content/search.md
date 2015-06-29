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
                },
                {
                    "count": 66,
                    "slug_value": "poynters",
                    "value": "Poynters"
                },
                {
                    "count": 1,
                    "slug_value": "steel-and-tube",
                    "value": "Steel & Tube"
                },
                {
                    "count": 1,
                    "slug_value": "urban-building-products",
                    "value": "Urban Building Products"
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
                },
                {
                    "count": 72,
                    "slug_value": "furniture-and-interiors",
                    "value": "Furniture & Interiors"
                },
                {
                    "count": 1,
                    "slug_value": "metal-timber-and-plastics",
                    "value": "Metal, Timber & Plastics"
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