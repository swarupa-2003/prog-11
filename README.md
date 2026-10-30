# Google Maps - Android Location Application

## Overview

Google Maps is an Android application developed using Kotlin and XML in Android Studio. The application demonstrates map display and location-based functionality using OpenStreetMap (OSM).

The application uses OpenStreetMap to display geographical maps without requiring a Google Maps API key or billing verification. It is designed to help users view map locations and understand how location services can be integrated into an Android application.

The application uses Android location services to obtain the device's current geographical location and provides a map-based interface for displaying location information.

## Aim

To develop an Android application that displays maps using OpenStreetMap and understand the implementation of location-based services in Android.

## Objectives

- To understand map integration in Android applications.
- To display geographical maps using OpenStreetMap.
- To implement location-based functionality.
- To understand Android LocationManager and LocationListener.
- To implement runtime permission handling for location access.
- To understand latitude and longitude coordinates.
- To design a user-friendly interface using XML layouts.

## Technologies Used

- **Programming Language:** Kotlin
- **User Interface:** XML
- **Development Environment:** Android Studio
- **Platform:** Android
- **Map Service:** OpenStreetMap (OSM)
- **Location Service:** Android LocationManager
- **Permissions:** ACCESS_FINE_LOCATION, ACCESS_COARSE_LOCATION, INTERNET
- **UI Components:** TextView, Button, LinearLayout
- **Map Display:** OpenStreetMap tiles

## Features

### 1. Map Display

Displays geographical maps using OpenStreetMap without requiring a Google Maps API key.

### 2. Current Location

Uses Android location services to obtain the device's current geographical coordinates.

### 3. Location Permissions

Requests the necessary location permissions from the user before accessing device location.

### 4. Latitude and Longitude

Uses geographical coordinates to identify the device's location.

### 5. Internet Connectivity

Uses internet permission to load map tiles from OpenStreetMap servers.

### 6. User-Friendly Interface

Provides a simple interface for viewing the map and accessing location-related functionality.

## Application Workflow

1. Launch the Google Maps application.
2. The application initializes the map interface.
3. OpenStreetMap map tiles are loaded using an internet connection.
4. The application checks whether location permissions have been granted.
5. If permission has not been granted, Android displays a runtime permission request.
6. After permission is granted, the application accesses Android location services.
7. The device's latitude and longitude are obtained when a location fix is available.
8. The application uses the coordinates to identify and display the current location on the map.

## Concepts Used

### 1. OpenStreetMap

OpenStreetMap is a free, open-source mapping platform that provides geographical map data.

The application uses OpenStreetMap tiles to display maps without requiring Google Maps API integration.

### 2. LocationManager

LocationManager is an Android system service used to obtain geographical location information.

It provides access to location providers such as GPS and network-based location.

### 3. LocationListener

LocationListener is used to receive location updates from the Android location service.

It helps the application respond when the device's geographical location changes.

### 4. Latitude and Longitude

Latitude and longitude are geographical coordinates used to identify a specific location on Earth.

- **Latitude:** Identifies the north-south position.
- **Longitude:** Identifies the east-west position.

### 5. Runtime Permissions

The application requests location permissions before accessing the device's location.

```xml
<uses-permission android:name="android.permission.ACCESS_FINE_LOCATION" />
<uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION" />
<uses-permission android:name="android.permission.INTERNET" />
```

### 6. Internet Permission

Internet permission allows the application to retrieve map tiles from OpenStreetMap servers.

### 7. OpenStreetMap Tiles

Map tiles are individual image sections that combine to display a complete geographical map. The application retrieves these tiles through an internet connection.

## Project Structure

```text
program11/
├── app/
│   └── src/
│       └── main/
│           ├── java/
│           │   └── com/
│           │       └── example/
│           │           └── program11/
│           │               └── MainActivity.kt
│           ├── res/
│           │   ├── drawable/
│           │   ├── layout/
│           │   │   └── activity_main.xml
│           │   └── values/
│           └── AndroidManifest.xml
├── README.md
└── build.gradle.kts
```

## Installation and Execution

1. Install Android Studio.
2. Clone or download the project repository.
3. Open the project in Android Studio.
4. Allow Gradle to sync and resolve dependencies.
5. Connect an Android device or start an emulator.
6. Ensure that internet connectivity is available.
7. Enable location services on the device or emulator.
8. Run the application.
9. Grant the requested location permissions.
10. Wait for the OpenStreetMap tiles and location information to load.

## Testing

| Test Case | Expected Result | Status |
|---|---|---|
| Launch application | Application screen is displayed | Pass |
| Load map | OpenStreetMap tiles are displayed | Pass |
| Internet connection | Map tiles load successfully | Pass |
| Grant location permission | Application can access location | Pass |
| Deny location permission | Appropriate permission message is displayed | Pass |
| Enable GPS | Device location can be obtained when a fix is available | Pass |
| Display coordinates | Latitude and longitude are retrieved | Pass |

## Screenshots

<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/c6fe7f2d-4b71-437a-8871-8f19dc0e0f25" />



## Learning Outcomes

- Understood map integration in Android applications.
- Learned to use OpenStreetMap for displaying geographical maps.
- Understood Android location services.
- Learned about LocationManager and LocationListener.
- Implemented runtime location permission handling.
- Understood latitude and longitude coordinates.
- Learned how internet connectivity is used to retrieve map tiles.
- Gained experience in developing Android applications using Kotlin and XML.

## Future Enhancements

- Add a search feature to find specific locations.
- Add zoom-in and zoom-out controls.
- Implement route navigation.
- Add markers for selected locations.
- Display the user's current location more accurately.
- Add distance calculation between two locations.
- Improve the interface and map interaction.

## Conclusion

The Google Maps Android application demonstrates map integration and location-based functionality using OpenStreetMap. It uses Android location services to obtain geographical coordinates and displays map information without requiring a Google Maps API key.

The application provides an understanding of OpenStreetMap, LocationManager, LocationListener, runtime permissions, and geographical coordinates. It demonstrates how map-based functionality can be implemented in Android using Kotlin and XML.

**Name:** swarupa s

**USN:** 25MCAR0137
