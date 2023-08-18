# vegas_map
Vegas Map

Note to self: when you want to update a dataset that is part of a qgis2web export, navigate to the "Data" folder and locate the .js file that corresponds to the data you're hoping to fix. Now replace the code with the .geojson code of your new dataset, but be sure to include

"var json_[file name] ="

...at the beginning. (In this example it's "var json_VegasHotelsandCasinosPolygons_1 = "). I guess this is to tell the file that it really is JavaScript. Also, feel free to reformat the first line to look nice and clean -- I think that helped me in this case.

ex. {"type": "FeatureCollection", "name": "Vegas Hotels and Casinos (Polygons)", "crs": { "type": "name", "properties": { "name": "urn:ogc:def:crs:OGC:1.3:CRS84" } }, "features": [ .......................
