<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Location Finder</title>
</head>
<body>
    <h1>Location Finder (Country, State, City, Town/Village)</h1>
    
    <button onclick="getLocation()">Get My Location Info</button>
    <div id="location-info" style="margin-top:20px;">
        <p><b>Country:</b> <span id="country">-</span></p>
        <p><b>State:</b> <span id="state">-</span></p>
        <p><b>City:</b> <span id="city">-</span></p>
        <p><b>Village/Town:</b> <span id="town">-</span></p>
    </div>

    <script>
        function getLocation() {
            if (navigator.geolocation) {
                navigator.geolocation.getCurrentPosition(showPosition, showError);
            } else {
                alert("Geolocation is not supported by this browser.");
            }
        }

        function showPosition(position) {
            const lat = position.coords.latitude;
            const lng = position.coords.longitude;

            const apiKey = 'AIzaSyCuIHb8y69apKtFG9yhydYf6CTphqEVmgk';
            const geocodeUrl = `https://maps.googleapis.com/maps/api/geocode/json?latlng=${lat},${lng}&key=${apiKey}`;

            fetch(geocodeUrl)
                .then(response => response.json())
                .then(data => {
                    if (data.status === "OK") {
                        const components = data.results[0].address_components;

                        let country = state = city = town = '-';

                        components.forEach(component => {
                            const types = component.types;
                            
                            if (types.includes('country')) {
                                country = component.long_name;
                            }
                            if (types.includes('administrative_area_level_1')) {
                                state = component.long_name;
                            }
                            if (types.includes('administrative_area_level_2')) {
                                city = component.long_name;
                            }
                            if (types.includes('locality') || types.includes('sublocality') || types.includes('neighborhood')) {
                                town = component.long_name;
                            }
                        });

                        document.getElementById('country').textContent = country;
                        document.getElementById('state').textContent = state;
                        document.getElementById('city').textContent = city;
                        document.getElementById('town').textContent = town;
                    } else {
                        alert('Unable to get location info');
                    }
                })
                .catch(error => {
                    console.error('Error fetching geocode:', error);
                });
        }

        function showError(error) {
            alert('Error getting location: ' + error.message);
        }
    </script>
</body>
</html>
