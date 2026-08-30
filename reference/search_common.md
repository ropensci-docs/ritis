# Search for tsn by common name

Search for tsn by common name

## Usage

``` r
search_common(x, from = "all", wt = "json", raw = FALSE, ...)
```

## Arguments

- x:

  text or taxonomic serial number (TSN) (character or numeric)

- from:

  (character) One of "all", "begin", or "end". See Details.

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

The `from` parameter:

- all - Search against the `searchByCommonName` API route, which
  searches entire name string

- begin - Search against the `searchByCommonNameBeginsWith` API route,
  which searches for a match at the beginning of a name string

- end - Search against the `searchByCommonNameEndsWith` API route, which
  searches for a match at the end of a name string

## See also

[`search_scientific()`](https://docs.ropensci.org/ritis/reference/search_scientific.md)

## Examples

``` r
if (FALSE) { # \dontrun{
search_common("american bullfrog")
search_common("ferret-badger")
search_common("polar bear")

# comparison: all, begin, end
search_common("inch")
search_common("inch", from = "begin")
search_common("inch", from = "end")

# end
search_common("snake", from = "end")
} # }
```
