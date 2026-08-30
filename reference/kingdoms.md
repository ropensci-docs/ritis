# Get kingdom names from tsn

Get kingdom names from tsn

## Usage

``` r
kingdom_name(tsn, wt = "json", raw = FALSE, ...)

kingdom_names(wt = "json", raw = FALSE, ...)
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

## Details

- kingdom_name: Get kingdom name for a TSN

- kingdom_names: Get all possible kingdom names

## Examples

``` r
if (FALSE) { # \dontrun{
kingdom_name(202385)
kingdom_name(202385, wt = "xml")
kingdom_names()
} # }
```
