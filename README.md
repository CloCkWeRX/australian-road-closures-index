# Australian Road Closures
An index of opencouncildata.org schema road closure feeds - typically from data.gov.au; though some sources require extra transformation.

Formats vary between CSV (with latitude, longitude to capture geometry) to geojson to shapefiles.


## Morph.io
Some of these datasets will require keys from morph.io - just sign up with your github account and programmatically populate the key param in the URL.

```
https://morph.io/CloCkWeRX/road-closures-morton-bay/data.csv?query=select+%2A+from+%27data%27&key=YOUR_KEY_HERE
```

## Contributing your data
Just open a pull request and add to sources.json

Country codes are aligned to: https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2

```
  "au": [{
    "name": "Morton Bay Regional Council",
    "wikidata_uri": "https://www.wikidata.org/wiki/Q1064985",
    "uri": "https://morph.io/CloCkWeRX/road-closures-morton-bay/data.csv?query=select+%2A+from+%27data%27&key=",
    "format": "text/csv",
    "schema": "http://standards.opencouncildata.org/#/road-closures"
  }]
```

Describing a publishing authority should be done with its wikidata identifier where possible; as this allows you to link to a spatial object (via openstreetmap) and a definitive topic (via wikipedia).



