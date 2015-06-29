# Productspec API V1

This is the official documentation for the Productspec API

API Objects
-----------

- [Authentication](content/authentication.md)
- [Primary Categories](content/categories.md)
- [Filter Products](content/search.md)
- [GET Product](content/product.md)

Making Requests
---------------

The base URL for all requsts is 'https://api.productspec.net/api/' Only https is supported.

The Productspec API uses HTTP Basic authentication

using cURL you would make a request like:

```shell
curl -u '<api_key>:x' https://api.productspec.net/search
```

Pagination
----------
Product search and filter results use pagination.  Each page has a limit of 25 products.  
To select select a page provide the 'page=<number>' querystring parameter.  The total number of available objects 
will be returned in the 'total' property

```shell
curl -u '<api_key>:x' https://api.productspec.net/search?page=2
```

