# Returns a list of the synonyms (if any) for the TSN.

Returns a list of the synonyms (if any) for the TSN.

## Usage

``` r
synonym_names(tsn, wt = "json", raw = FALSE, ...)
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

a data.frame

## Examples

``` r
if (FALSE) { # \dontrun{
synonym_names(tsn=183671) # tsn not accepted
synonym_names(tsn=526852) # tsn accepted
} # }
```
