# DiscoveryFit
DiscoveryFit is a mobile app designed for treasure hunts, designed as walking routes with key points that participants must record using NFC devices.
Two user roles are available: player and administrator. Administrators can create and modify activities, register players for them, and monitor their progress.
Players, meanwhile, can participate in assigned activities, following the route on the map and interacting with NFC devices located along the way. The journeys will be recorded using the device's GPS location.

This project is my final year project for my degree in Computer Engineering. It continues the work started in a project from the previous year, from which I use the database and the system API.

DiscoveryFit is an Android mobile application developed in Java, using Gradle as the build system. It uses the Retrofit library for API connectivity and OSMdroid for map management. It also uses the external OpenRouteService API for route calculation and coordinate translation.

Author: Sonia Gallego Trapero [SoniaGaTr](https://github.com/SoniaGaTr)

Tutor: Raúl Alonso Calvo [raulalonsoc](https://github.com/raulalonsoc)

*⚠️ NOTE: The original repository containing the code is private, but I want to share the README and the final report of my TFG.⚠️*

## Table of Contents

* [Download project](#download-project)
* [Technologies](#technologies)
* [Project organization](#project-organization)
* [How to use](#how-to-use)

## Download project ##
### Prerequisites ###
- [Java JDK](<https://www.oracle.com/java/technologies/javase-downloads.html>) (versión 8 o superior)

### Instructions ###
1. Clone the git repsitory:  `git clone https://github.com/raulalonsoc/DiscoveryFit.git`
2. Open the project in Android Studio.
3. Ensure dependencies are configured in build.gradle.
4. Build and run the app on a physical device or emulator.

## Technologies ##
* Language: Java
* Build System: Gradle
* Platform: Android

## Project organization ##

The project is organized into the following main directories and files:

* `app`
  * `java/es.upm.etssinf.gib.discoveryfitn`: Contains the core Java classes for the app.
    * `activities`: Includes Activity classes, such as MainActivity and LoginActivity.
        * `admin`: Contains the activities corresponding to the administrator's functionalities.
        * `player`: Contains the activities corresponding to the player's functionalities.
    * `adapters`: Holds the adapter classes for managing the display of recipe lists.
    * `models`: Contains model classes to represent the data structure and the adapter classes for managing the display of lists.
        * `Api`: 
        * `ORSApi`: 
    * `Utils`: 
  * `res`
    * `layout`: XML files for UI layouts.
    * `values`: Resources for consistent styling and colors.
        * `strings`:
    * `drawable`: Holds images and icons used within the app.
    * `navigation`: 

## How to use ##
When you open the app, the login screen appears, and you can also access the user log in. Once you log in, the main screen corresponding to the user role appears: player or administrator. The session remains open unless the user logs out.

Administrators will be able to create and modify activities—defining the information, route, and associated NFC devices—register players for those activities, and monitor their progress.

Players, meanwhile, will be able to view and participate in the activities they have been registered for. When starting an activity, a map is displayed; players must follow the route and register NFC devices located at key points along the way. They can also view and modify their user information.

You can find a demo video of the application at: 
