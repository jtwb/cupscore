CUP Score
=========

**Cumulative Unpainted Pixel Score** is a partial implementation of Meenan's [Speed Index](https://sites.google.com/a/webpagetest.org/docs/using-webpagetest/metrics/speed-index). **Speed Index** is a heuristic for the sensation of interface snappiness.

* `cup-wpt-framegrab` - download all frames from a webpagetest result by `xmlUrl`.
* `cup-compare` - render all changed pixels as black
* `cup-magnitude` - return number of black pixels in image

Uses [webpagetest](http://www.webpagetest.org/), [cURL](http://curl.haxx.se/), [Image Magick](https://github.com/trevor/ImageMagick).

Usage:
```sh
cup-wpt-framegrab 130612_TE_1D76
cup-compare lastframe.jpg someframe.jpg | cup-magnitude
```
