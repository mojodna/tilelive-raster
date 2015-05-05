# tilelive-raster

I am a [tilelive](https://github.com/mapbox/tilelive.js) source for simple
rasters, both local and remote.

## Usage

This is intended for RGB(A) multiband rasters. It uses Mapnik (via
tilelive-mapnik) and GDAL (via node-gdal) under the hood to inspect rasters and
render them, so it should work with any format that GDAL supports (and has been
compiled with support for).

```javascript
// fetch a remote raster (it will be cached in $TMPDIR and cleaned up when the
// process exits)
tilelive.load("raster+http://example.com/whatever.tif", ...);

// generate tiles from a local raster
tilelive.load("raster+file://./whatever.tif", ...);
```
