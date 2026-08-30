# ITIS Solr facet

ITIS Solr facet

## Usage

``` r
itis_facet(..., proxy = NULL, callopts = list())
```

## Arguments

- ...:

  Arguments passed on to the `params` parameter of the
  [`solrium::solr_facet()`](https://rdrr.io/pkg/solrium/man/solr_facet.html)
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

## Examples

``` r
if (FALSE) { # \dontrun{
itis_facet(q = "rank:Species", rows = 0, facet.field = "kingdom")$facet_fields

x <- itis_facet(q = "hierarchySoFar:*$Aves$* AND rank:Species AND usage:valid",
   facet.pivot = "nameWInd,vernacular", facet.limit = -1, facet.mincount = 1,
   rows = 0)
head(x$facet_pivot$`nameWInd,vernacular`)
} # }
```
