# Returns the scientific name for the TSN. Also returns the component parts (names and indicators) of the scientific name.

Returns the scientific name for the TSN. Also returns the component
parts (names and indicators) of the scientific name.

## Usage

``` r
scientific_name(tsn, wt = "json", raw = FALSE, ...)
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
scientific_name(tsn = 531894)
} # }
```
