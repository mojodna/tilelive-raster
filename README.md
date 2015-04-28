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

## Caveats

If you need support for JPEG-compressed GeoTIFFs (until
[naturalatlas/node-gdal#101](https://github.com/naturalatlas/node-gdal/issues/101)
is fixed), use the following for a source build of node-gdal:

```bash
npm install --build-from-source=gdal
```

This can be used when installing `tilelive-raster` or when installing dependent
modules for an app or library that requires `tilelive-raster`.
