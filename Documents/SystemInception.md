# System Inception

## Table of Contents
* Requirements
  * [Functional Requirements](#functional-requirements)
  * [Nonfunctional Requirements](#nonfunctional-requirements)
  * [Security Requirements](#security-requirements)

## Requirements

<a name="functional-requirements" />
### Functional Requirements
The following actors and use cases have been identified for the Ozarks Day Hiker application.

![image](https://raw.githubusercontent.com/wildharpo/ozarks-day-hiker-app/refs/heads/main/Documents/Diagrams/UseCaseDiagram.jpg)

This diagram represents the following use cases:

* Browse Hikes - A *Hiker* looks at a list of hikes, which contains the name of the hike, the length of the hike, and a short description of the hike.
* Read About a Hike - A *Hiker* reads a detailed description of a hike they have selected.
* View Hike on Map - A *Hiker* views the route of the trail on a map. In addition to a route of the trail, points of interest are indicated on the map.
* Find Driving Directions - A *Hiker* reads general directions to a trail head. It is also possible to get detailed directions to a trail head based upon the *Hiker's* current location.
* Watch Trail Videos - A *Hiker* selects and views a video of the trail. Videos may describe a hike, part of a hike, POI along the trail, or other subjects related to the trail.
* View Hike on Google Earth - A *Hiker* views the trail route and POIs on Google Earth.
* Leave a Comment on a Hike - A *Hiker* leaves a comment about the trail, a POI, or an associated subject.
* Read Hike Comments - A *Hiker* reads the comments on the hike posted by others.
* Setup a Hike in GPS Trail Guide Mode - A *Hiker* downloads the information necessary to use the app without a data connection on their mobile device.
* Use GPS Trail Guide Mode - A *Hiker* views the hike map, POIs, and their current position on a map without a data connection. A *Hiker's* current position is continuously updated on the map.
* Create a Trail Entry - A *Hike Admin* creates the entry for a new trail to be included in the trails featured on the app.
* Edit a Trail Entry - A *Hike Admin* makes corrections to the text in a trail entry; adds or deletes additional pictures; adds or deletes POI; or adds or deletes videos.

<a name="nonfunctional-requirements" />
### Nonfunctional Requirements
* Hikers will be able to easily interact with the ODHkr App on a variety of devices. This applies to all use cases associated with the *Hiker* actor.
* The hike map will be readable and scrollable on common cell phone and tablet devices. This applies to the following use cases - View Hike on Map, Use GPS Trail Guide Mode.
* The GPS location will be accurate to within 10 feet of the actual locations. This applies to the following use case - Use GPS Trail Guide Mode.

<a name="security-requirements" />
### Security Requirements
* Data exchanged between the Hike Admin and the ODHkr system will be encrypted. This applies to all use cases associated with the *Hike Admin* role.
* Scripts will not be allowed in user input. This applies to the following use case - Leave a Comment on a Hike.
