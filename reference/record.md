# Gets a record from an LSID

Gets a record from an LSID

## Usage

``` r
record(lsid, wt = "json", raw = FALSE, ...)
```

## Arguments

- lsid:

  lsid for a taxonomic group (character). Required.

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

## Details

Gets the partial ITIS record for the TSN in the LSID, found by comparing
the TSN in the search key to the TSN field. Returns an empty result set
if there is no match or the TSN is invalid.

## Examples

``` r
if (FALSE) { # \dontrun{
record(lsid = "urn:lsid:itis.gov:itis_tsn:180543")
} # }
```
