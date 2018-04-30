# Changes

## v0.5.0 - 4/30/18

* Upgrade `@mapbox/mapnik-omnivore` to prevent duplicate Mapnik versions when
  installed with other, newer libs.

## v0.4.2 - 6/14/17

* Fix dependency `require`s

## v0.4.1 - 6/13/17

* Request `@mapbox/tilelive-mapnik` as a peer dependency

## v0.4.0 - 6/13/17

* Upgrade dependencies for compatibility with node-6.x+

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
