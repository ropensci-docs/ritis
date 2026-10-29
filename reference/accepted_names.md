# Get accepted names from tsn

Get accepted names from tsn

## Usage

``` r
accepted_names(tsn, wt = "json", raw = FALSE, ...)
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

Zero row data.frame if the name is accepted, otherwise a data.frame with
information on the currently accepted name

## Examples

``` r
if (FALSE) { # \dontrun{
# TSN accepted - good name, empty data.frame returned
accepted_names(tsn = 208527)

# TSN not accepted - input TSN is old name, non-empty data.frame returned
accepted_names(tsn = 504239)

# raw json
accepted_names(tsn = 208527, raw = TRUE)
} # }
```
