# Get ITIS terms, i.e., tsn's, authors, common names, and scientific names

Get ITIS terms, i.e., tsn's, authors, common names, and scientific names

## Usage

``` r
terms(query, what = "both", wt = "json", raw = FALSE, ...)
```

## Arguments

- query:

  One or more common or scientific names, or partial names

- what:

  One of both (search common and scientific names), common (search just
  common names), or scientific (search just scientific names)

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
# Get terms searching both common and scientific names
terms(query='bear')

# Get terms searching just common names
terms(query='tarweed', "common")

# Get terms searching just scientific names
terms(query='Poa annua', "scientific")

# many at once
terms(query=c('Poa annua', 'Pinus contorta'), "scientific")
} # }
```
