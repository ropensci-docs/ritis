# Provides the date the ITIS database was last updated

Provides the date the ITIS database was last updated

## Usage

``` r
last_change_date(wt = "json", raw = FALSE, ...)
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

character value with a date

## Examples

``` r
if (FALSE) { # \dontrun{
last_change_date()
last_change_date(wt = "xml")
} # }
```
