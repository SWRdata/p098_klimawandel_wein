# README

## Before you start

All data was added to the `.gitignore` and uploaded to OneDrive. Copy all folders from the [OneDrive data directory](https://suedwestrundfunk.sharepoint.com/:f:/r/sites/SWRDATA/Freigegebene%20Dokumente/p098_klimawandel_wein/data?csf=1&web=1&e=TBMJ5B) to `src/data/raw`.


## Working with NETCDF files

Raw data comes in the `NETCDF` file format which provides a lightweight, multidimensional data structure. The downside is you'll need to get used to it, especially when you're more used to working with two-dimensional csvs or traditional geojson/vector data.

Wihtin the `R` ecosystem, there are a couple packages that deal with `NETCDF` data. In my expericence, the `stars` package provides the most intuitive and powerful API. It was written by Edzer Pebesma, a spatial statistician based in Münster who also authored the ubiquitious `sf` package. A good introduction can be found in the book ["Spatial Data Science"](https://r-spatial.org/book/07-Introsf.html#package-stars). 