google-map-highlighter
=====
##Summary##
The `google-map-highlighter` Polymer component creates a  [google-map](https://github.com/GoogleWebComponents/google-map) with a marker in the centre at the place to be highlighted.
It auto-generates a layout for the marker's infowindow based on the information given by the placeId which can be used or personal formatting can be used instead (or a combination).


####Examples####
Using placeId and the auto generated info window.
```
<google-map-highlighter placeId="ChIJN1t_tDeuEmsRUsoyG83frY4">
	Your extra information goes in here.
</google-map-highlighter>
```

Using an address and overwriting the name.
```
<google-map-highlighter address="48 Pirrama Road, Pyrmont, NSW" name="Google, Sydney" details="false">
</google-map-highlighter>
```

Allowing directions.
```
<google-map-highlighter placeId="ChIJN1t_tDeuEmsRUsoyG83frY4" name="Google, Sydney" enableDirections="true">
</google-map-highlighter>
```

With apiKey.
```
<google-map-highlighter apiKey="abc123" placeId="ChIJN1t_tDeuEmsRUsoyG83frY4" name="Google, Sydney">
</google-map-highlighter>
```
##Attributes##
#### Required *(one of the following)* ####

**placeId** The place to be highlighted.

**address** The address of the place to be highlighted (overwritten by placeId, if it is also given.)

#### Optional ####

**zoom**
  The initial zoom of the map.
  *default: 14*
  
**name**
  The name to be shown in the infowindow and on hover over the marker.
  *default: the name given in the placeId*
  
**apiKey**
  Your Google Maps API Key.
  *default: null*
  
**enableDirections**
  Whether or not to show a search box at the top of the map so that people can get directions to the location being highlighted.
  *default: false*
  
**details**
  Whether or not to generate information for the infowindow from the place_id.
  *default: true*

