# Get global species completeness from tsn

Get global species completeness from tsn

## Usage

``` r
global_species_completeness(tsn, wt = "json", raw = FALSE, ...)
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
global_species_completeness(tsn = 180541)
global_species_completeness(180541, wt = "xml")
global_species_completeness(180541, wt = "json", raw = TRUE)
} # }
```
