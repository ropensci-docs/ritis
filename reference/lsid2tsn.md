# Gets the TSN corresponding to the LSID, or an empty result if there is no match.

Gets the TSN corresponding to the LSID, or an empty result if there is
no match.

## Usage

``` r
lsid2tsn(lsid, wt = "json", raw = FALSE, ...)
```

## Arguments

- lsid:

  (character) lsid for a taxonomic group. Required.

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
lsid2tsn(lsid="urn:lsid:itis.gov:itis_tsn:28726")
lsid2tsn(lsid="urn:lsid:itis.gov:itis_tsn:28726", wt = "xml")
lsid2tsn("urn:lsid:itis.gov:itis_tsn:0")
lsid2tsn("urn:lsid:itis.gov:itis_tsn:0", wt = "xml")
} # }
```
