Product
==========

Get Product
----------------------

 - `GET /api/product/4e7002604ff399d11457cd39` will return the product with the ID of `4e7002604ff399d11457cd39`.
 
**Product Model**
```json
{
    "company_email": "cedarspec@jsctimber.co.nz",
    "company_id": "48717cb74ff399d11457bc60",
    "company_logo_url": "https://ps-content.s3.amazonaws.com/company/48717cb74ff399d11457bc60/logo/jsc-timber-logo.jpg",
    "company_name": "JSC Timber",
    "company_phone": "09 412 2800",
    "company_slug": "jsc-timber",
    "product_description": "<p>Board and Batten is a vertical design created using wide clear cedar boards spaced apart with narrow battens covering the joints, as per NZS E2/AS1 PROFILES to NZS 3617/BRANZ BULLETIN 411. There are no set limitations on widths and various combinations are used to create different looks with the most common being 6x1 and 8x1 Boards covered with 3x1 Battens. This can also be reversed with boards installed over Battens to create a deep negative channel effect.</p>",
    "product_id": "4e7002604ff399d11457cd39",
    "product_images": [
        {
            "large_path": "https://ps-content.s3.amazonaws.com/product/4e7002604ff399d11457cd39/images/4e7002a14ff39ad1cc0562a2/00335web-lg.jpg",
            "medium_path": "https://ps-content.s3.amazonaws.com/product/4e7002604ff399d11457cd39/images/4e7002a14ff39ad1cc0562a2/00335web-md.jpg",
            "small_path": "https://ps-content.s3.amazonaws.com/product/4e7002604ff399d11457cd39/images/4e7002a14ff39ad1cc0562a2/00335web-sm.jpg"
        },
        {
            "large_path": "https://ps-content.s3.amazonaws.com/product/4e7002604ff399d11457cd39/images/4e7002d74ff39ad1cc0562a3/goh-house-crown-range-053-w-lg.jpg",
            "medium_path": "https://ps-content.s3.amazonaws.com/product/4e7002604ff399d11457cd39/images/4e7002d74ff39ad1cc0562a3/goh-house-crown-range-053-w-md.jpg",
            "small_path": "https://ps-content.s3.amazonaws.com/product/4e7002604ff399d11457cd39/images/4e7002d74ff39ad1cc0562a3/goh-house-crown-range-053-w-sm.jpg"
        },
        {
            "large_path": "https://ps-content.s3.amazonaws.com/product/4e7002604ff399d11457cd39/images/4e7002f44ff39ad1cc0562a4/goh-house-crown-range-003-w-lg.jpg",
            "medium_path": "https://ps-content.s3.amazonaws.com/product/4e7002604ff399d11457cd39/images/4e7002f44ff39ad1cc0562a4/goh-house-crown-range-003-w-md.jpg",
            "small_path": "https://ps-content.s3.amazonaws.com/product/4e7002604ff399d11457cd39/images/4e7002f44ff39ad1cc0562a4/goh-house-crown-range-003-w-sm.jpg"
        },
        {
            "large_path": "https://ps-content.s3.amazonaws.com/product/4e7002604ff399d11457cd39/images/4e70030f4ff39ad1cc0562a5/goh-house-crown-range-006-lg.jpg",
            "medium_path": "https://ps-content.s3.amazonaws.com/product/4e7002604ff399d11457cd39/images/4e70030f4ff39ad1cc0562a5/goh-house-crown-range-006-md.jpg",
            "small_path": "https://ps-content.s3.amazonaws.com/product/4e7002604ff399d11457cd39/images/4e70030f4ff39ad1cc0562a5/goh-house-crown-range-006-sm.jpg"
        }
    ],
    "product_slug": "jsc-board-and-batten-weatherboard-system",
    "product_tech_files": [
        {
            "_id": "4f3881b34ff399d11457f064",
            "file_ext": ".pdf",
            "file_group": "General",
            "file_name": "JSC Timber Profile Booklet"
        },
        {
            "_id": "4f3881c94ff399d11457f065",
            "file_ext": ".pdf",
            "file_group": "General",
            "file_name": "Board & Batten Direct Fixed Details"
        },
        {
            "_id": "4f38821b4ff399d11457f066",
            "file_ext": ".pdf",
            "file_group": "General",
            "file_name": "JSC Nail Profiles"
        }
    ],
    "product_title": "JSC Board & Batten Weatherboard System"
}
```

**Product Model Properties**

| Property | Description |
| -------- | ------------ |
| `product_id` | ID of product|
| `company_id` | ID of company|
| `company_name` | company name|
| `company_logo_url` | url of logo|
| `product_title` | name of the product|
| `product_slug` | slugged name of the product|
| `company_slug` | slugged name of the company|
| `company_phone` | contact phone number of company|
| `company_email` | contact email of company|
| `product_description` | description of the product HTML encoded|
| `product_images` | Array of image paths for this product.  each image object has URL for small, medium, and large versions|
| `product_tech_files` | array of technical files for this product (see model description below)|

**Product Technial File Properties**

| Tech File Property | Description |
| -------- | ------------ |
| `_id` | ID of technical file - used to retrieve technial file|
| `file_ext` | file extension|
| `file_group` | group name of this technial file (e.g., warranty, BRANZ, GreenTag, etc...)|
| `file_name` | name of technial file|



**Status Codes**
- `200 OK` will be returned if query is successful
- `404 Not Found` will be returned if product is not found




Get Technical File
------------------

- `GET /api/techfile/4e7002604ff399d11457cd39/4f3881b34ff399d11457f064` 
request for URL of the product technical file where `4e7002604ff399d11457cd39` is the product id and `4f3881b34ff399d11457f064` is the id of the technial file




