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
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

