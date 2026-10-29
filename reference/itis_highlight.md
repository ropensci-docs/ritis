# ITIS Solr highlight

ITIS Solr highlight

## Usage

``` r
itis_highlight(..., proxy = NULL, callopts = list())
```

## Arguments

- ...:

  Arguments passed on to the `params` parameter of the
  [`solrium::solr_highlight()`](https://rdrr.io/pkg/solrium/man/solr_highlight.html)
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
itis_highlight(q = "rank:Species", hl.fl = 'rank', rows=10)
} # }
```
