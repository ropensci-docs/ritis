# Get all possible geographic values

Get all possible geographic values

## Usage

``` r
geographic_values(wt = "json", raw = FALSE, ...)
```

## Arguments

- wt:

  (character) One of "json" or "xml". Required.

- raw:

  (logical) Return raw JSON or XML as character string. Required.
  Default: `FALSE`

- ...:

  curl options passed on to
  [crul::HttpClient](https://docs.ropensci.org/crul/reference/HttpClient.html)

## Value

character vector of geographic names

## Examples

``` r
if (FALSE) { # \dontrun{
geographic_values()
geographic_values(wt = "xml")
geographic_values(wt = "json", raw = TRUE)
} # }
```
