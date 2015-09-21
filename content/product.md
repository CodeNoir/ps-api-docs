Product
==========

Get Product
----------------------

 - `GET /api/product/4e7002604ff399d11457cd39` will return the product with the ID of `4e7002604ff399d11457cd39`.
 
 **Optional Querystring Parameters**

| Parameter | Value |
| -------- | ------------ |
| `casestudy` | Use `?casestudy=0` to not include case studies when retrieving a product.|
| `cads` | Use `?cads=0` to not include CAD files when retrieving a product. |
 
 ```
 `GET /api/product/4e7002604ff399d11457cd39?cads=0&casestudy=0` 
 Retrieves a product without any CAD files or case studies.
```

**Product Model** 
```json
{
    "product_id": "4e9b90464ff399d11457cd6a",
    "product_title": "Colt Euro Seefire",
    "product_slug": "colt-euro-seefire",
    "company_id": "462f03184ff399d11457b737",
    "company_name": "Colt Products & Systems",
    "company_logo_url": "https://ps-content.s3.amazonaws.com/company/462f03184ff399d11457b737/logo/logo.png",
    "company_phone": "04 913 2072",
    "company_email": "coltnz@aquaheat.co.nz",
    "company_slug": "colt-products-and-systems",
    "product_range": "Colt Natural &amp; Smoke Ventilators",
    "product_description": "<p>Colt Euro Seefire is a natural louvred ventilator that is available in a wide range of sizes, louvre options and control options. It is suited to most industrial and commercial buildings and can provide both day to day and smoke ventilation, as well as permit the entry of natural daylight if fitted with glass or polycarbonate blades. Colt Euro Seefire can also be installed in the vertical either for low level air inlet or for high level extract. With the addition of optional extras it can provide year round weathered ventilation.</p><p>Colt Euro Seefire is manufactured to the ISO 9000 quality standard.</p>",
    "product_images": [
        {
            "large_path": "https://ps-content.s3.amazonaws.com/product/4e9b90464ff399d11457cd6a/images/4f5fb36a4ff39ad1cc056306/dsc00705-lg.JPG",
            "medium_path": "https://ps-content.s3.amazonaws.com/product/4e9b90464ff399d11457cd6a/images/4f5fb36a4ff39ad1cc056306/dsc00705-md.JPG",
            "small_path": "https://ps-content.s3.amazonaws.com/product/4e9b90464ff399d11457cd6a/images/4f5fb36a4ff39ad1cc056306/dsc00705-sm.JPG"
        },
        {
            "large_path": "https://ps-content.s3.amazonaws.com/product/4e9b90464ff399d11457cd6a/images/4f5fb3724ff39ad1cc056307/dsc00697-lg.JPG",
            "medium_path": "https://ps-content.s3.amazonaws.com/product/4e9b90464ff399d11457cd6a/images/4f5fb3724ff39ad1cc056307/dsc00697-md.JPG",
            "small_path": "https://ps-content.s3.amazonaws.com/product/4e9b90464ff399d11457cd6a/images/4f5fb3724ff39ad1cc056307/dsc00697-sm.JPG"
        }
    ],
    "product_tech_files": [
        {
            "_id": "4e9b90904ff399d11457ef3d",
            "file_ext": ".pdf",
            "file_group": "General",
            "file_name": "Wellington Hospital"
        },
        {
            "_id": "518711e24ff399d11457fc01",
            "file_ext": ".pdf",
            "file_group": "General",
            "file_name": "Seefire natural ventilator"
        }
    ],
    "product_compliance_docs": [
        {
            "_id": "518711e24ff399d11457fc01",
            "file_ext": ".pdf",
            "file_group": "BRANZ",
            "file_name": "BRANZ example"
        }
    ],
    "product_environmental_docs": [
    {
            "_id": "518711e24ff399d11457fa23",
            "file_ext": ".pdf",
            "file_group": "GreenTag",
            "file_name": "Green Tag example"
        }
    ],
    "product_cads": [
        {
            "file_name": "euro-sf-1225-curb-02",
            "file_preview_url": "https://ps-content.s3.amazonaws.com/cad/4fbc64fd4ff39ad1cc05a452/files/4fbc64fd4ff39ad1cc05a452/euro-sf-1225-curb-02_dwg.jpg",
            "file_types": [
                {
                    "_id": "4fbc64fd4ff39ad1cc05a452",
                    "file_extension": ".dwg"
                }
            ],
            "group_name": "Outside Louvre"
        },
        {
            "file_name": "euro-sf-1819-wall-02",
            "file_preview_url": "https://ps-content.s3.amazonaws.com/cad/4fbc68a44ff39ad1cc05a453/files/4fbc68a44ff39ad1cc05a453/euro-sf-1819-wall-02_dwg.jpg",
            "file_types": [
                {
                    "_id": "4fbc68a44ff39ad1cc05a453",
                    "file_extension": ".dwg"
                }
            ],
            "group_name": "Outside Louvre"
        }
    ],
    "product_videos": [
        {
            "vimeo_url": "",
            "youtube_url": "http://www.youtube.com/v/EH9_0I2waPA&context=C32e72c5ADOEgsToPDskIb6-CsZ9vb5TMK-It1wnS1&hl=en&fs=1&rel=0"
        }
    ],
    "product_case_studies": [
        {
            "_id": "52b105a94ff399d114580b3f",
            "city": "Auckland City",
            "description": "<p>Possibly the largest penthouse louvre in the world! A Colt Universal 3UL Triple Bank Louvre System 10x10mx10m, takes pride of place on top of one of the most ground breaking buildings in New Zealand.  <br>In an effort to reduce ASB\u2019s carbon footprint by 20%, and set new standards for environmental quality and energy performance, ASB has taken full advantage of some of the latest sustainable systems and building technologies. <br>This is Australasia\u2019s first fixed-bin, displacement, mixed mode ventilation system.  This complex ventilation system utilizes thermal mass and the Venturi effect to extract heat from the building and exhaust it through the internal funnel like atria and out via Colt\u2019s chimney-like penthouse louvre.  <br>The Colt triple bank louvres are used to protect the actuated dampers located in behind which open depending on wind direction, effectively \u2018dragging\u2019 heat load from the building. This passive ventilation system is then controlled by an internal computer system.  <br>Colt\u2019s 3UL/DH louvre system was specified for maximum rain defence, aerodynamics and guaranteed performance tested in accordance with AS/NZS 4740:2000.<br>Colt Products and Systems were contracted to design, manufacture and install the high performance weather louvre system with a BMS actuated damper structure behind and all of the secondary structural steel for the cube. National Manager for Colt Products and Systems, Andy Oakley says \u201cOur engineers were instrumental with the design and construction methodology of the cube at a very early stage\u201d.   <br>Internationally, Colt is a front runner in sustainable technology. Colt develops technologies that harness the natural elements to make the most efficient use of energy, and contribute to a sustainable built environment.</p>",
            "images": [
                {
                    "full_src": "https://ps-content.s3.amazonaws.com/case-study-image/52b105aa4ff399d114580cb0/asb-north-wharf.jpg",
                    "icon_src": "https://ps-content.s3.amazonaws.com/case-study-image/52b105aa4ff399d114580cb0/asb-north-wharf_thumb.jpg",
                    "position": "https://ps-content.s3.amazonaws.com/undefined"
                },
                {
                    "full_src": "https://ps-content.s3.amazonaws.com/case-study-image/52b105aa4ff399d114580cb1/asb-the-cube.jpg",
                    "icon_src": "https://ps-content.s3.amazonaws.com/case-study-image/52b105aa4ff399d114580cb1/asb-the-cube_thumb.jpg",
                    "position": "https://ps-content.s3.amazonaws.com/undefined"
                }
            ],
            "participants": [
                {
                    "job_title": "Architectural Designer",
                    "name": "BVN & Jasmax"
                },
                {
                    "job_title": "Contractor",
                    "name": "Fletcher Construction Ltd"
                }
            ],
            "project_type": "Commercial",
            "title": "ASB North Wharf"
        }
    ],
    "warranties" : [
		{
			"warranty_title" : "BUILDING PRODUCT WARRANTY – RESIDENTIAL",
			"description" : "Firth Industries warrants that Firth Structural and Architectural Masonry Products will for a period of 10 years from the date of purchase:\n• be free from defects outside the acceptable limits specified in NZS4210 and AS/NZS4455 due to factory workmanship or materials\nused in manufacturing the product; and\n• subject to compliance with the conditions attached, that the products will perform to the extent set out in the relevant Firth Industries published literature current at the time of installation.\n\nThis warranty is subject to the storage, installation and maintenance requirements and the other warranty conditions set out in this\ndocument.\nTexture and colour variation due to the natural material used can occur in masonry products and is not deemed a product defect.\nMinor chipping, cracking, or efflorescence is also not deemed a product defect when evaluated and deemed compliant with the Firth\nArchitectural Best Practice Guide.\nNothing in this warranty shall exclude or modify any legal rights a customer may have under the Consumer Guarantees Act 1993 or otherwise which cannot be excluded or modified by law.",
			"warranty_has_doc" : true,
			"how_to_claim" : "Contact supplier.",
			"exclusions" : "No exclusions.",
			"validity_period_months" : 120,
			"_id" : "55ff3648a379b3216ed738b3",
			"maintenance" : [
				{
					"description" : "This warranty is subject to Structural and Architectural Masonry products being properly stored, installed and maintained in accordance with the Firth Masonry Home Construction Manual, the Firth Architectural Best Practice Guide and the Firth Structural and Architectural Masonry Product Technical Statement.",
					"_id" : "55ff3648a379b3216ed738b4",
					"frequency_months" : 24
				}
			]
		}
	]
}
```

**Product Model Properties**

| Property | Description |
| -------- | ------------ |
| `product_id` | ID of product.|
| `product_title` | Name of the product.|
| `product_slug` | Slugged name of the product.|
| `company_id` | ID of company.|
| `company_name` | Company name.|
| `company_logo_url` | URL of logo.|
| `company_phone` | Contact phone number of company.|
| `company_email` | Contact email of company.|
| `company_slug` | Slugged name of the company.|
| `product_range` | Name of the range to which this product belongs.|
| `product_description` | Description of the product HTML encoded.|
| `product_images` | Array of image paths for this product. Each image object has a URL for small, medium, and large versions.|
| `product_tech_files` | Array of technical files for this product. (See model description below.)|
| `product_compliance_docs` | Array of compliance files for this product. (See model description below.)|
| `product_environmental_docs` | Array of supporting environmental files for this product. (See model description below.)|
| `product_cads` | Array of supporting CAD files for this product. (See model description below.)|
| `product_videos` | Array of supporting YouTube or Vimeo URLs for this product. (See model description below.)|
| `product_case_studies` | Array of case studies where this product has been used. (See model description below.)|


**Product Technical File, Compliance Docs, and Environmental Properties**

| Tech File Property | Description |
| -------- | ------------ |
| `_id` | ID of the file. (Used to retrieve the file.)|
| `file_ext` | File extension.|
| `file_group` | Group name of this file. (e.g., warranty, BRANZ, GreenTag, etc.)|
| `file_name` | Name of the file.|



**Product CADS**

| CAD Property | Description |
| -------- | ------------ |
| `file_name` | Name of the file.|
| `file_preview_url' | URL of the preview image for this CAD file. |
| `group_name` | Name of the group to which this CAD file belongs. |
| `file_types` | Array of _ids and extensions for this CAD file. (Note that a single CAD file may have many different file types.) |
| `file_ext` | File extension.|
| `file_group` | Group name of this file. (e.g., warranty, BRANZ, GreenTag, etc.)|


| CAD file_types Property | Description |
| -------- | ------------ |
| `file_extension` | Type of file (dwg, pdf, rfa, etc.).|
| `_id` | The ID of the CAD file extension. use this _id to download the file. (see below.)|



**Product Case Studies**

| Case Study Property | Description |
| -------- | ------------ |
| `_id` | ID of the case study.|
| `title` | The title of the case study. |
| `city' | City location of the case study. |
| `description` | Description of the case study. (HTML encoded.) |
| `project_type` | Type of project that this case study relates to. |
| `participants` | Array of all the participants related to this case study. (see below.)|
| `images` | Array of images for this case study. (see below.)|
| 

| Case Study Participants Property | Description |
| -------- | ------------ |
| `job_title` | Job title of the participant. |
| `name` | Name of the participant. |

| Case Study Images Property | Description |
| -------- | ------------ |
| `job_title` | Job title of the participant. |
| `name` | Name of the participant. |


**Product Videos**

| Product Videos Property | Description |
| -------- | ------------ |
| `vimeo_url` | Returns a Vimeo URL or an empty string if a URL does not exist. |
| `youtube_url` | Returns a YouTube URL or an empty string if a URL does not exist. |


**Status Codes**
- `200 OK` will be returned if query is successful.
- `404 Not Found` will be returned if a product was not found.





Download File (CAD, Technical, Compliance, Environmental)
---------------------------------------------------------

- `GET /api/file/key/[YourApiKey]/[FileType]/[FileId]` will either return the file requested or a 404 if file is not found.

| Property | Description |
| -------- | ------------ |
| `YourApiKey` | Your API key provided to you by Productspec. |
| `FileType` | `tech` or `cad` (all files other than CAD files are considered tech). |
| `FileId` | The ID of the file being requested. |















































