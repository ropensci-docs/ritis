# Search by scientific name

Search by scientific name

## Usage

``` r
search_scientific(x, wt = "json", raw = FALSE, ...)
```

## Arguments

- x:

  text or taxonomic serial number (TSN) (character or numeric)

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

## See also

[`search_common`](https://docs.ropensci.org/ritis/reference/search_common.md)

## Examples

``` r
if (FALSE) { # \dontrun{
search_scientific("Tardigrada")
search_scientific("Quercus douglasii")
} # }
```
