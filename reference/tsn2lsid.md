# Gets the unique LSID for the TSN, or an empty result if there is no match.

Gets the unique LSID for the TSN, or an empty result if there is no
match.

## Usage

``` r
tsn2lsid(tsn, wt = "json", raw = FALSE, ...)
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

a character string, an LSID, or `NULL` if nothing found

## Examples

``` r
if (FALSE) { # \dontrun{
tsn2lsid(tsn = 155166)
tsn2lsid(tsn = 333333333)
tsn2lsid(155166, raw = TRUE)
tsn2lsid(155166, wt = "xml")
} # }
```
