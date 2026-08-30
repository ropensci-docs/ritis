# Get tsn by vernacular language

Get tsn by vernacular language

## Usage

``` r
tsn_by_vernacular_language(language, wt = "json", raw = FALSE, ...)
```

## Arguments

- language:

  A string containing the language. This is a language string, not the
  international language code (character)

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
tsn_by_vernacular_language(language = "french")
} # }
```
