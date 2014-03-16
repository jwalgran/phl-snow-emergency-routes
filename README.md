# Philadelphia Snow Emergency Routes

A web map of Philadelphia's snow emergency routes.

[View the map](http://jwalgran.github.io/phl-snow-emergency-routes)

From the [Streets Department snow emergency route page](http://www.philadelphiastreets.com/highways/snow/emergency-routes/) 

> When snow accumulations approach emergency status, the Managing Director may declare a snow emergency. Once emergency status is declared, the City's 110 miles of Snow Emergency Routes receive priority. Owners of vehicles and dumpsters must move them to alternate parking spaces so City forces can clear snow from curb-to-curb on the emergency routes. Any vehicle remaining on a Snow Emergency Route during the declared Snow Emergency will be ticketed and towed. If your car is towed, call 215-686-SNOW for its location. Do NOT call 911.

The
[snow-emergency-routes.csv](https://github.com/jwalgran/phl-snow-emergency-routes/blob/master/snow-emergency-routes.csv)
file was created from the table on the
[Streets Department snow emergency route page](http://www.philadelphiastreets.com/highways/snow/emergency-routes/).
I used this file to generate the
[snow-emergency-route-segment-ids.csv](https://github.com/jwalgran/phl-snow-emergency-routes/blob/master/snow-emergency-route-segment-ids.csv) file.


The
[snow-emergency-route-segment-ids.csv](https://github.com/jwalgran/phl-snow-emergency-routes/blob/master/snow-emergency-route-segment-ids.csv)
file contains the IDs of all of the
street segments that are classified as snow emergency routes. The snow
emergency routes shapefile/geojson is built by filtering the
[street centerline layer](https://github.com/CityOfPhiladelphia/phl-open-geodata/tree/master/street_centerline)
to include only those rows where the `seg_id` is contained in this list.
