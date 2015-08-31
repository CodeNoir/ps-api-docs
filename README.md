# Productspec API V1

This is the official documentation for the Productspec API

API Objects
-----------

- [Primary Categories](content/categories.md)
- [Filter Products](content/search.md)
- [GET Product](content/product.md)

Making Requests
---------------

The base URL for all requsts is 'https://api.productspec.net/' Only https is supported.

The Productspec API uses an API key that must be included in an custom HTTP request header named 'api-key'
-- The Productspec API key is used only for identification purposes and is not private.  Future versions of this API may require a private key, but for now it is public.

using cURL you would make a request like:

```shell
curl -H 'api-key: <api_key>' -XGET 'https://api.productspec.net/api/product/4e9b90464ff399d11457cd6a'
```
`*Exception: requests for files must include the api-key in the url not header*`


Pagination
----------
Product search and filter results use pagination.  Each page has a limit of 25 products.  
To select select a page provide the 'page=<number>' querystring parameter.  

```shell
curl -H 'api-key: <api_key>' https://api.productspec.net/api/search?page=2
```

The total number of available objects will be returned in the 'total' property on the results object returned.

