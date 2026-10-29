# ITIS Solr search

ITIS Solr search

## Usage

``` r
itis_search(..., proxy = NULL, callopts = list())
```

## Arguments

- ...:

  Arguments passed on to the `params` parameter of the
  [`solrium::solr_search()`](https://rdrr.io/pkg/solrium/man/solr_search.html)
  function. See
  [solr_fields](https://docs.ropensci.org/ritis/reference/solr_fields.md)
  for possible parameters, and examples below

- proxy:

  List of arguments for a proxy connection, including one or more of:
  url, port, username, password, and auth. See
  [`crul::proxy()`](https://docs.ropensci.org/crul/reference/proxies.html)
  for help, which is used to construct the proxy connection.

- callopts:

  Curl options passed on to
  [crul::HttpClient](https://docs.ropensci.org/crul/reference/HttpClient.html)

## Details

The syntax for this function can be a bit hard to grasp. See
https://itis.gov/solr_examples.html for help on generating the syntax
ITIS wants for specific searches.

## References

<https://www.itis.gov/solr_documentation.html>

## Examples

``` r
if (FALSE) { # \dontrun{
itis_search(q = "tsn:182662")

# get all orders within class Aves (birds)
z <- itis_search(q = "rank:Class AND nameWOInd:Aves")
hierarchy_down(z$tsn)

# get taxa "downstream" from a target taxon
## taxize and taxizedb packages have downstream() fxns, but
## you can do a similar thing here by iteratively drilling down
## the taxonomic hierarchy
## here, we get families within Aves
library(data.table)
aves <- itis_search(q = "rank:Class AND nameWOInd:Aves")
aves_orders <- hierarchy_down(aves$tsn)
aves_families <- lapply(aves_orders$tsn, hierarchy_down)
rbindlist(aves_families)

# the tila operator
itis_search(q = "nameWOInd:Liquidamber\\ styraciflua~0.4")

# matches only monomials
itis_search(q = "nameWOInd:/[A-Za-z0-9]*[ ]{0,0}*/")

# matches only binomials
itis_search(q = "nameWOInd:/[A-Za-z0-9]*[ ]{1,1}[A-Za-z0-9]*/")

# matches only trinomials
itis_search(q = "nameWOInd:/[A-Za-z0-9]*[ ]{1,1}[A-Za-z0-9]*[ ]{1,1}[A-Za-z0-9]*/")

# matches binomials or trinomials
itis_search(q = "nameWOInd:/[A-Za-z0-9]*[ ]{1,1}[A-Za-z0-9]*[ ]{0,1}[A-Za-z0-9]*/")

itis_search(q = "nameWOInd:Poa\\ annua")

# pagination
itis_search(q = "nameWOInd:/[A-Za-z0-9]*[ ]{0,0}*/", rows = 2)
itis_search(q = "nameWOInd:/[A-Za-z0-9]*[ ]{0,0}*/", rows = 200)

# select fields to return
itis_search(q = "nameWOInd:/[A-Za-z0-9]*[ ]{0,0}*/",
   fl = c('nameWInd', 'tsn'))
} # }
```
