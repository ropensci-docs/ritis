# Get jurisdictional origin from tsn

Get jurisdictional origin from tsn

## Usage

``` r
jurisdictional_origin(tsn, wt = "json", raw = FALSE, ...)

jurisdiction_origin_values(wt = "json", raw = FALSE, ...)

jurisdiction_values(wt = "json", raw = FALSE, ...)
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

- jurisdictional_origin: data.frame

- jurisdiction_origin_values: data.frame

- jurisdiction_values: character vector

## Details

Jurisdiction methods:

- jurisdictional_origin: Get jurisdictional origin from tsn

- jurisdiction_origin_values: Get jurisdiction origin values

- jurisdiction_values: Get all possible jurisdiction values

## Examples

``` r
if (FALSE) { # \dontrun{
jurisdictional_origin(tsn=180543)
jurisdictional_origin(tsn=180543, wt = "xml")

jurisdiction_origin_values()

jurisdiction_values()
} # }
```
