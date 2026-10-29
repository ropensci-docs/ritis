# Get hierarchy down from tsn

Get hierarchy down from tsn

## Usage

``` r
hierarchy_down(tsn, wt = "json", raw = FALSE, ...)

hierarchy_up(tsn, wt = "json", raw = FALSE, ...)

hierarchy_full(tsn, wt = "json", raw = FALSE, ...)
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

## Details

Hierarchy methods:

- hierarchy_down: Get hierarchy down from tsn

- hierarchy_up: Get hierarchy up from tsn

- hierarchy_full: Get full hierarchy from tsn

## Examples

``` r
if (FALSE) { # \dontrun{
## Full down (class Mammalia)
hierarchy_down(tsn=179913)

## Full up (genus Agoseris)
hierarchy_up(tsn=36485)

## Full hierarchy
### genus Liatris
hierarchy_full(tsn=37906)
### get raw data back
hierarchy_full(tsn=37906, raw = TRUE)
### genus Baetis, get xml back
hierarchy_full(100800, wt = "xml")
} # }
```
