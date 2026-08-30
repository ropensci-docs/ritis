# Get common names from tsn

Get common names from tsn

## Usage

``` r
common_names(tsn, wt = "json", raw = FALSE, ...)
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

a data.frame

## Examples

``` r
if (FALSE) { # \dontrun{
common_names(tsn=183833)
common_names(tsn=183833, wt = "xml")
} # }
```
