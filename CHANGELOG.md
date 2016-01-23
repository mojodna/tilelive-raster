# Changes

## v0.3.0 - 1/22/16

* Upgrade to `mapnik-omnivore@^7.1.0` (w/ `gdal@0.8.0` + binaries for node-5.x)

## v0.2.2 - 6/11/15

* Improve debugging capabilities using `debug`. To enable, set
  `DEBUG=tilelive-raster`
* Require `tilelive-error` correctly

## v0.2.1 - 5/6/15

* Update to `mapnik-omnivore@6.0.0` (w/ `gdal@0.4.4`) and remove `gdal`
  dependency

## v0.2.0 - 5/5/15

* Update to `node-gdal@0.4.4` w/ JPEG and DEFLATE support
* Use `tilelive-error` to prevent repeated attempts to load unsuitable rasters

## v0.1.2 - 5/4/15

* Attach a `close()` handler to clean up tmp files

## v0.1.1 - 4/30/15

* Improve the default zoom

## v0.1.0 - 4/27/15

* Initial release
