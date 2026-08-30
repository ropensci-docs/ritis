# Provides a list of the unique languages used in the vernacular table.

Provides a list of the unique languages used in the vernacular table.

## Usage

``` r
vernacular_languages(wt = "json", raw = FALSE, ...)
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

a character vector of verncular names

## Examples

``` r
if (FALSE) { # \dontrun{
vernacular_languages()
} # }
```
