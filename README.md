# Google Maps Location Tracker - Android Application

## Overview
This Android application displays a map with markers for your current location and a destination, along with a polyline connecting the two points. It uses Google Maps API and the Fused Location Provider to get the user's current location.

## Features
- Displays an interactive Google Map
- Shows your current location (if permissions are granted)
- Marks a predefined destination location
- Draws a line between your location and the destination
- Handles location permissions gracefully

## Prerequisites
- Android Studio
- Android device or emulator with Google Play Services
- Google Maps API key (already included in the manifest)

## Installation
1. Clone this repository
2. Open the project in Android Studio
3. Build and run the application on your device or emulator

## Code Structure
### Main Files:
- `MainActivity.java`: Contains the main logic for displaying the map and handling location
- `AndroidManifest.xml`: Contains permissions and API key configuration

### Key Components:
- Google Maps API integration
- Fused Location Provider for getting device location
- Permission handling for location access
- Map markers and polylines

## Usage
1. Launch the application
2. Grant location permissions when prompted
3. The map will display:
   - A blue dot showing your current location (if available)
   - A marker at the destination (Bascom Hill, Madison, WI)
   - A line connecting your location to the destination

## Customization
To change the destination location:
1. Modify the `mDestinationLatLng` variable in `MainActivity.java`
2. Update the coordinates to your desired location

Example:
```java
private final LatLng mDestinationLatLng = new LatLng(YOUR_LATITUDE, YOUR_LONGITUDE);
```

## Permissions
The app requires the following permissions:
- `ACCESS_FINE_LOCATION` - For precise location data
- `ACCESS_COARSE_LOCATION` - For approximate location data
- `INTERNET` - For accessing Google Maps services

These are already declared in the AndroidManifest.xml file.

## Known Issues
- Location might not update in real-time (uses last known location)
- Requires Google Play Services to be installed on the device

## Screenshot
<img width="1440" height="3120" alt="image" src="https://github.com/user-attachments/assets/96bdf01e-93e5-4b5c-a8c5-ed90d1ee3e1c" />

