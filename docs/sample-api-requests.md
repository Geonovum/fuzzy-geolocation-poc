# Sample OGC API requests

*NOTE: Work in progress*

## References
[OGC API Features backgrounds and specification](https://ogcapi.ogc.org/features/)

## Demo API for the fuzzy geolocation PoC
Base url / landing page: [http://inspirelab.geonovum.nl/ogcapifeatures/](http://inspirelab.geonovum.nl/ogcapifeatures/)

This API supports JSON and HTML encodings, which makes browsing through the API quite easy.

Just give it a try :).

### API definition
Get the Open API definition from:
* [http://inspirelab.geonovum.nl/ogcapifeatures/openapi](http://inspirelab.geonovum.nl/ogcapifeatures/openapi)

Use content negotiation for JSON or HTML encoded documents. Or direct links (easier for exploring the API):
* [Open API (JSON)](http://inspirelab.geonovum.nl/ogcapifeatures/openapi?f=json)
* [Open API (HTML)](http://inspirelab.geonovum.nl/ogcapifeatures/openapi?f=html)

### Explore API
To see what data is avalaible, see the list of collections:

http://inspirelab.geonovum.nl/ogcapifeatures/collections

The API offers 1 collection now: "RD info stations", available at:
http://inspirelab.geonovum.nl/ogcapifeatures/collections/rdinfostations

which provides more data (metadata) about this collection

TODO: sample response in JSON

### Get data
After exploring the API and data available, you could easily construct the requests to get data by adding the `/items` part at the end:

http://inspirelab.geonovum.nl/ogcapifeatures/collections/rdinfostations/items

### Paging through the data
- changing the `limit` gives more/less items
- using the `next` links enables browsing through the data


### Get data using a boundingbox (area of interest)
Sample requests:
- http://inspirelab.geonovum.nl/ogcapifeatures/collections/rdinfostations/items?bbox=5.8,52.1,6.1,52.4&f=json
- http://inspirelab.geonovum.nl/ogcapifeatures/collections/rdinfostations/items?bbox=5.8,52.1,6.1,52.4
