# Plugin development directory

This is where all code development should be done.  Run `pb_tool
deploy` to deploy into `..\SurvexImport`.  The contents of that
directory can then be copied to the QGIS3 python plugin directory.
This can either be done by hand or by running `make install` in the
top level directory.

### Extra python scripts

* `dump3d.py` replicates _exactly_ the functionality of the survex
  `dump3d` command in pure python, for debugging.

* `test3d.py` was used for debugging the treatment of the passage wall
  data.  It runs like `dump3d.py`, but additionally generates a number of
  `*.dat` files containing xy data which can be read into a standard
  plotting package.

* `old3d2json.py` converts old-style ASCII .3d files at v0.01 to
  GeoJSON, writing to stdout, and optionally adding a CRS.
