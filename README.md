whereonearth-building
==

_Forking GeoPlanet one place type a time._

This is an active but still experimental project to create a community-driven
project to maintain and update the Creative Commons licensed GeoPlanet dataset.

Rather than create a single repository with every record the plan is to create
smaller datasets organized by placetype in the hopes that they will be more
manageable to download and to update by users interested in particular place types.

Each location (building) is stored as a separate GeoJSON file. GeoJSON was
chosen because it has wide support in variety of GIS tools, most programming
languages (and specifically JavaScript), can be edited using any old text editor
(or Github's own "edit this page" functionality) and allows for any number of
custom key/value pairs using the GeoJSON _properties_ dictionary.

The naming convention for records is the building's Where On Earth (WOE) ID
followed by a ".json" extension. Records are stored in nested directories that
correspond to their WOE ID. The top level directory would be the first three
digits of a WOE ID, the second level directory would be the following three
digits (four through six) and so on until their are no more digits in the WOE
ID. For example, given the WOE ID ID 2147595424 the full path of the record
would be: [214/759/542/4/2147595424.json](https://github.com/straup/whereonearth-building/blob/master/data/214/759/542/4/2147595424.json)

Technically buildings are not part of the GeoPlanet hierarchy but they should be
and so since the [building=yes](http://buildingequalsyes.spum.org/) project has
already reverse-geocoded most of the 26 million buildings present in the
[OpenStreetMap](http://www.openstreetmap.org) project so we'll just start with
those.

Currently only buildings parented by
[airports](https://github.com/straup/whereonearth-airport) are included in this
repository.

See also
--

* [whereonearth-airport](https://github.com/straup/whereonearth-airport/)

* [building=yes](http://buildingequalsyes.spum.org/)

* [woe.spum.org](http://woe.spum.org)

* [GeoPlanet data downloads](http://developer.yahoo.com/geo/geoplanet/data/)
