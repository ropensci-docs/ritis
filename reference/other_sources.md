# Returns a list of the other sources used for the TSN.

Returns a list of the other sources used for the TSN.

## Usage

``` r
other_sources(tsn, wt = "json", raw = FALSE, ...)
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

## Examples

``` r
if (FALSE) { # \dontrun{
# results
other_sources(tsn=182662)
# no results
other_sources(tsn=2085272) 
# get xml
other_sources(tsn=182662, wt = "xml")
} # }
```
