# Provides a list of all the unique rank names contained in the database and their kingdom and rank ID values.

Provides a list of all the unique rank names contained in the database
and their kingdom and rank ID values.

## Usage

``` r
rank_names(wt = "json", raw = FALSE, ...)
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

a data.frame, with columns:

- kingdomname

- rankid

- rankname

## Examples

``` r
if (FALSE) { # \dontrun{
rank_names()
} # }
```
