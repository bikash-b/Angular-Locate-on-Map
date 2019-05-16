# Angular-Locate-on-Map
![alt text](https://github.com/bikash-b/Angular-Locate-on-Map/blob/master/locate-on-map.png)

Angular loate on map or "locate-on-map" is the component to display the Google map with a search box where user can search any place and locate the place on the map.

## How to use

### Step 1

First download the component to your project directory and declare the component in the NgModule. If you have only AppModule then just declare in the AppModule else declare in any feature module.

### Step 2

Get the Google API Key to use the map. Once you get the key, then include the below script in your index.html.

*<script async defer src="https://maps.googleapis.com/maps/api/js?key=YOUR_API_KEY&callback=initMap" type="text/javascript"></script>*

### Step 3

Now you are ready to use the component. In any of your component template just call the selector i.e *<locate-on-map></locate-on-map>*.

## Component attributes

| Attribute name| Description   | Value |
| ------------- |:-------------:| -----:|
| markerHeight      | To change the marker height. It accepts number. | Positive number e.g 20, 30, 50 |
| markerWidth      | To change the marker height. It accepts number. | Positive number e.g 20, 30, 50 |
| markerIcon      | To change the default marker icon. It accepts string which holds the image URL. | Image URL e.g *http://localhost:4200/assets/marker.png* |
| moreOptions      | To provide the additional features in the apps icon on the search box. It accepts array of strings | Array of strings e.g ["Change input color", "Get place info"] |
| defaultPosition      | To provide the default position to the map. It accepts MapPosition. | MapPosition e.g lattitude, longitude, zoom |
| displayInfoWindow      | To display the Information Window on click on the marker. It is a boolean. | Boolean e.g true or false |
| displayMoreOption      | To display the More Option on the Search box. It is a boolean. | Boolean e.g true or false |
| infoWindowHeaderAlign      | To provide the allignment to the default InfoWindow header. It accepts string. | String e.g 'left' or 'center' or 'right'|
| displayAddressOnInfoWindow      | right-aligned | $1600 |
| displayOpenHoursOnInfoWindow      | right-aligned | $1600 |
| displayRatingsOnInfoWindow      | right-aligned | $1600 |
| displayReviewOnInfoWindow      | right-aligned | $1600 |
| displayContactOnInfoWIndow      | right-aligned | $1600 |
| isInfoWindowCustomizable      | right-aligned | $1600 |
| isMoreOptionCustomizable      | right-aligned | $1600 |

