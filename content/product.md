Product
==========

Get Product
----------------------

 - `GET /api/product/4db64faa4ff399d11457cbff` will return the product with the ID of 4db64faa4ff399d11457cbff.
 

```json
{
    "company_email": "info@poynters.co.nz",
    "company_id": "4a96f2664ff399d11457bcf1",
    "company_logo_url": "https://ps-content.s3.amazonaws.com/company/4a96f2664ff399d11457bcf1/logo/logo.png",
    "company_name": "Poynters",
    "company_phone": "0800 769 683",
    "company_slug": "poynters",
    "product_description": "<p>Patio dining arm chair from Poynters.</p><p>Our \"Patio\" outdoor dining arm chair is a supremely comfortable chair for use either as a dining chair or as a general use armchair. A deep skirt but rounded edges creates a chair of unique appearance.</p><p>Woven by hand in ecolene synthetic fineweave wicker in a lovely, soft broken white colour for a touch of warmth and a nice breezy style that is like a breath of fresh air.</p><p>The chair is finished in 2mm fineweave woven around a quality powdercoated aluminium frame.</p><p>Price includes cushion pad finished in taupe outdoor durable fabric and Quickdry Foam branded all-weather foam  - the market leader.</p><p>Colour is broken white.</p>",
    "product_id": "4db64faa4ff399d11457cbff",
    "product_images": [
        {
            "large_path": "https://ps-content.s3.amazonaws.com/product/4db64faa4ff399d11457cbff/images/4db64fd94ff39ad1cc0560ee/dsc01215__75146_zoom-lg.JPG",
            "medium_path": "https://ps-content.s3.amazonaws.com/product/4db64faa4ff399d11457cbff/images/4db64fd94ff39ad1cc0560ee/dsc01215__75146_zoom-md.JPG",
            "small_path": "https://ps-content.s3.amazonaws.com/product/4db64faa4ff399d11457cbff/images/4db64fd94ff39ad1cc0560ee/dsc01215__75146_zoom-sm.JPG"
        }
    ],
    "product_slug": "patio-dining-arm-chair",
    "product_tech_files": [],
    "product_title": "Patio dining arm chair"
}
```

| Property | Description |
| -------- | ------------ |
| `total: number` | Total number of products found for the query (25 results returned per request)|
| `products: array of products` | Products found matching the query |
| `filters: array` | The filters array contains all filters that match the query provided.  Use the `slug_value` and `filter_key` to build query|

**Status Codes**
- `200 OK` will be returned if query is successful
- `404 Not Found` will be returned if product is not found


