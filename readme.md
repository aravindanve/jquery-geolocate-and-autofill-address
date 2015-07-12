# Geolocate and Autofill Address using Google Maps API

#### by [Aravindan Ve](http://github.com/aravindanve)

## Requires

* jQuery
* Google Maps JavaScript API

        <script src="https://maps.googleapis.com/maps/api/js?v=3.exp&signed_in=true&libraries=places"></script>

## Usage

* Include the script `location-autocomplete.js` 

* Initialize after document ready:

        var autolocation = new LocationAutocomplete('input-id-to-autocomplete', {

            // fills in only the listed components
            'target-autofill-input-1': {components: ['administrative_area_level_1:long_name', 'country:short_name']},

            // fills in all the address components returned by google maps api
            'target-autofill-input-2': {components: ['_all:long_name']},

        }, 'auto-locate-button-id');
