# Returns the usage information for the TSN.

Returns the usage information for the TSN.

## Usage

``` r
usage(tsn, wt = "json", raw = FALSE, ...)
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
usage(tsn = 526852)
usage(tsn = 526852, raw = TRUE)
usage(tsn = 526852, wt = "xml")
} # }
```
