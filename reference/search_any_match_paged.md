# Search for any matched page

Search for any matched page

## Usage

``` r
search_any_match_paged(
  x,
  pagesize = NULL,
  pagenum = NULL,
  ascend = NULL,
  wt = "json",
  raw = FALSE,
  ...
)
```

## Arguments

- x:

  text or taxonomic serial number (TSN) (character or numeric)

- pagesize:

  An integer containing the page size (numeric)

- pagenum:

  An integer containing the page number (numeric)

- ascend:

  A boolean containing true for ascending sort order or false for
  descending (logical)

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

a data.frame

## See also

[`search_anymatch`](https://docs.ropensci.org/ritis/reference/search_anymatch.md)

## Examples

``` r
if (FALSE) { # \dontrun{
search_any_match_paged(x=202385, pagesize=100, pagenum=1, ascend=FALSE)
search_any_match_paged(x="Zy", pagesize=100, pagenum=1, ascend=FALSE)
} # }
```
