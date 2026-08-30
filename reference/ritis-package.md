# ritis

Interface to Integrated Taxonomic Information (ITIS)

## ritis package API

All functions that start with `itis_` work with the ITIS Solr API
described at <https://www.itis.gov/solr_documentation.html>, which uses
the package solrium, and these functions have you use the solrium
function interfaces, so you can pass on parameters to the solrium
functions - so the solrium docs are important here.

All other functions work with the ITIS REST API described at
<https://www.itis.gov/ws_description.html>. For these methods, they can
grab data in either JSON or XML format. JSON is the default. We parse
the JSON to R native format, either data.frame, character string, or
list. You can get raw JSON as a character string back, or raw XML as a
character string, and then parse yourself with jsonlite or xml2

You'll also be interested in the taxize book <https://taxize.dev/>

## Terminology

- "mononomial": a taxonomic name with one part, e.g, *Poa*

- "binomial": a taxonomic name with two parts, e.g, *Poa annua*

- "trinomial": a taxonomic name with three parts, e.g, *Poa annua annua*

## Author

Scott Chamberlain <myrmecocystus@gmail.com>
