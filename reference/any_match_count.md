# Get any match count.

Get any match count.

## Usage

``` r
any_match_count(x, wt = "json", raw = FALSE, ...)
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

An integer containing the number of matches the search will return.

## Examples

``` r
if (FALSE) { # \dontrun{
any_match_count(x = 202385)
any_match_count(x = "dolphin")
any_match_count(x = "dolphin", wt = "xml")
} # }
```
