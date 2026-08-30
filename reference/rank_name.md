# Returns the kingdom and rank information for the TSN.

Returns the kingdom and rank information for the TSN.

## Usage

``` r
rank_name(tsn, wt = "json", raw = FALSE, ...)
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

a data.frame, with rank name and other info

## Examples

``` r
if (FALSE) { # \dontrun{
rank_name(tsn = 202385)
} # }
```
