# Get credibility rating from tsn

Get credibility rating from tsn

## Usage

``` r
credibility_rating(tsn, wt = "json", raw = FALSE, ...)

credibility_ratings(wt = "json", raw = FALSE, ...)
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

## Details

methods:

- credibility_rating: Get credibility rating for a tsn

- credibility_ratings: Get possible credibility ratings

## Examples

``` r
if (FALSE) { # \dontrun{
credibility_rating(tsn = 526852)
credibility_rating(526852, wt = "xml")
credibility_rating(526852, raw = TRUE)

credibility_ratings()
credibility_ratings(wt = "xml")
credibility_ratings(raw = TRUE)
} # }
```
