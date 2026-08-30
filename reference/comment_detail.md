# Get comment detail from TSN

Get comment detail from TSN

## Usage

``` r
comment_detail(tsn, wt = "json", raw = FALSE, ...)
```

## Arguments

- tsn:

  TSN for a taxonomic group (numeric). Required.

- wt:

  (character) One of "json" or "xml". Required.

- raw:

  (logical) Return raw JSON or XML as character string. Required.
  Default: `FALSE`

- ...:

  curl options passed on to
  [crul::HttpClient](https://docs.ropensci.org/crul/reference/HttpClient.html)

## Value

A data.frame with results.

## Examples

``` r
if (FALSE) { # \dontrun{
comment_detail(tsn=180543)
comment_detail(tsn=180543, wt = "xml")
} # }
```
