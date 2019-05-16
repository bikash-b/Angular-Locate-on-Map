# Angular Locate on Map
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

| Attribute     | Description   | Value |
| ------------- |:-------------:| -----:|
| markerHeight      | To change the marker height. It accepts number. | Positive number e.g 20, 30, 50 |
| markerWidth      | To change the marker height. It accepts number. | Positive number e.g 20, 30, 50 |
| markerIcon      | To change the default marker icon. It accepts string which holds the image URL. | Image URL e.g *http://localhost:4200/assets/marker.png* |
| moreOptions      | To provide the additional features in the apps icon on the search box. It accepts array of strings | Array of strings e.g ["Change input color", "Get place info"] |
| defaultPosition      | To provide the default position to the map. It accepts MapPosition. | MapPosition e.g lattitude, longitude, zoom |
| displayInfoWindow      | To display the Information Window on click on the marker. It is a boolean. | Boolean e.g true or false |
| displayMoreOption      | To display the More Option on the Search box. It is a boolean. | Boolean e.g true or false |
| infoWindowHeaderAlign      | To provide the allignment to the default InfoWindow header. It accepts string. | String e.g 'left' or 'center' or 'right'|
| displayAddressOnInfoWindow      | To display the Addess on the default InfoWindow. It accepts boolean. | Boolean e.g true or false |
| displayOpenHoursOnInfoWindow      | To display the Opening Hours on the default InfoWindow. It accepts boolean. | Boolean e.g true or false |
| displayRatingsOnInfoWindow      | To display the Ratings on the default InfoWindow. It accepts boolean. | Boolean e.g true or false |
| displayReviewOnInfoWindow      | To display the Review on the default InfoWindow. It accepts boolean. | Boolean e.g true or false |
| displayContactOnInfoWIndow      | To display the Contact information on the default InfoWindow. It accepts boolean. | Boolean e.g true or false |
| isInfoWindowCustomizable      | To customize the InfoWindow on the map. It accepts boolean. | Boolean e.g true or false |
| isMoreOptionCustomizable      | To customize the more option placed near the search box. It accepts boolean. | Boolean e.g true or false |

## Component events

| Event         | Description   | Return |
| ------------- |:-------------:| -----:|
| onOpenInfoWindow      | It triggers when the InfoWindow loaded to the map. | Value of type *InfoWindowEvent* |
| onMoreOptionClick      | It triggers on click of the option available in the more optionsection near search box. | Value of type *MoreOptionEvent* |
| onComponentLoad      | It triggers when component loaded to the browser. | Value of type *ComponentLoadEvent* |

## How to set the attributes

Following code snippet show how to set the attributes to the component i.e *<locate-on-map>*,
  
        <locate-on-map [mapConfig]="mapConfig"></locate-on-map>
        
In your component class define and assign the values to *mapConfig*, where *mapConfig* is type of *MapConfig*,

        mapConfig: MapConfig  = {
          defaultPosition: this.defaultMapPosition,
          markerHeight: 60,
          markerWidth: 60,
          displayInfoWindow: true,
          displayMoreOption: true,
          infoWindowHeaderAlign: "center",
          displayOpenHoursOnInfoWindow: true,
          displayRatingsOnInfoWindow: true,
          displayReviewOnInfoWindow: true,
          displayAddressOnInfoWindow: true,
          displayContactOnInfoWIndow: true,
          isInfoWindowCustomizable: true,
          moreOptions: ["Change input color", "Custom option1", "Custom option2"]
        }
        
## Demo

Please find the demo link i.e [https://angular-locate-on-map-1-1umiuq.stackblitz.io/](https://angular-locate-on-map-1-1umiuq.stackblitz.io/).
