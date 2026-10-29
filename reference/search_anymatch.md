# Search for any match

Search for any match

## Usage

``` r
search_anymatch(x, wt = "json", raw = FALSE, ...)
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

[`search_any_match_paged`](https://docs.ropensci.org/ritis/reference/search_any_match_paged.md)

## Examples

``` r
if (FALSE) { # \dontrun{
search_anymatch(x = 202385)
search_anymatch(x = "dolphin")
# no results
search_anymatch(x = "Pisces")
} # }
```
