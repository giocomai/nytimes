<!-- README.md is generated from README.Rmd. Please edit that file -->



<!-- badges: start -->
[![Travis build status](https://travis-ci.org/news-r/nytimes.svg?branch=master)](https://travis-ci.org/news-r/nytimes)
<!-- badges: end -->

# nytimes

The goal of `nytimes` is to integrate all of the [New York Times API](https://developer.nytimes.com) with R.

## Installation

``` r
#install.packages("remotes")
remotes::install_github("news-r/nytimes")
```

## APIs

- [x] [Archive](https://developer.nytimes.com/docs/archive-product/1/overview) 
- [ ] [Article Search](https://developer.nytimes.com/docs/articlesearch-product/1/overview)
- [ ] [Books](https://developer.nytimes.com/docs/books-product/1/overview)
- [ ] [Geo](https://developer.nytimes.com/docs/geo-product/1/overview)
- [ ] [Most Popular](https://developer.nytimes.com/docs/most-popular-product/1/overview)
- [ ] [Most Reviews](https://developer.nytimes.com/docs/movie-reviews-api/1/overview)
- [ ] [Semantic](https://developer.nytimes.com/docs/semantic-api-product/1/overview)
- [ ] [Times Tags](https://developer.nytimes.com/docs/timestags-product/1/overview)
- [ ] [Times Wire](https://developer.nytimes.com/docs/timeswire-product/1/overview)
- [ ] [Top Stories](https://developer.nytimes.com/docs/top-stories-product/1/overview)

## Setup

First, [create an account](https://developer.nytimes.com) to obtain an API key. Then either specify the aforementioned key using `nytimes_key` or specify it as environment variable (likely in your `.Renviron`) as `NYTIMES_API_KEY`.

```r
library(nytimes)

ny_key("xXxxX")
```

## Examples


```r
library(nytimes)

# get all articles from January first 2018
archive <- ny_archive(2018, 1)
```
