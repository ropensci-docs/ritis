# Get description of the ITIS service

Get description of the ITIS service

## Usage

``` r
description(wt = "json", raw = FALSE, ...)
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

a string, the ITIS web service description

## Examples

``` r
if (FALSE) { # \dontrun{
description()
description(wt = "xml")
} # }
```
