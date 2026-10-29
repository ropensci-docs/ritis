# Returns a list of the pulications used for the TSN.

Returns a list of the pulications used for the TSN.

## Usage

``` r
publications(tsn, wt = "json", raw = FALSE, ...)
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
publications(tsn = 70340)
publications(tsn = 70340, wt = "xml")

publications(tsn = 70340, verbose = TRUE)
} # }
```
