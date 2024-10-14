# System Inception

## Table of Contents
* Requirements
  * [Functional Requirements](#functional-requirements)
  * [Nonfunctional Requirements](#nonfunctional-requirements)
  * [Security Requirements](#security-requirements)
* [Technology Plan](#technology-plan)
* Risk Analysis
  * [Technical Risk by Business Goal](#technical-risk-by-business-goal)
  * [Risk Mitigation Plan](#risk-mitigation-plan)

## Requirements

<div name="functional-requirements">
  <h3>Functional Requirements</h3>
</div>
The following actors and use cases have been identified for the Ozarks Day Hiker application.

#### Actors
| Actor | Description |
|-------|-------------|
| Hiker | A *Hiker* is a person who uses the app to explore day hikes in the Ozarks or who uses the app to actually take a day hike. |
| Hiker Admin | A *Hike Admin* is a person who can add new hikes to the list of featured day hikes. They can also modify an existing hike. Note that a Hike Admin can use the app as a Hiker would and is thus a Hiker. A Hiker, however, is not a Hike Admin |

#### Use Cases
![image](https://raw.githubusercontent.com/wildharpo/ozarks-day-hiker-app/refs/heads/main/Documents/Diagrams/UseCaseDiagram.jpg)

This diagram represents the following user stories:

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

<div name="nonfunctional-requirements">
  <h3>Nonfunctional Requirements</h3>
</div>
The following nonfunctional requirements will be satisfied.

* Hikers will be able to easily interact with the ODHkr App on a variety of devices. This applies to all use cases associated with the *Hiker* actor.
* The hike map will be readable and scrollable on common cell phone and tablet devices. This applies to the following use cases - View Hike on Map, Use GPS Trail Guide Mode.
* The GPS location will be accurate to within 10 feet of the actual locations. This applies to the following use case - Use GPS Trail Guide Mode.

<div name="security-requirements">
  <h3>Security Requirements</h3>
</div>
The following security requirements will be satisfied.

* Data exchanged between the Hike Admin and the ODHkr system will be encrypted. This applies to all use cases associated with the *Hike Admin* role.
* Scripts will not be allowed in user input. This applies to the following use case - Leave a Comment on a Hike.

<div name="technology-plan">
  <h2>Technology Plan</h2>
</div>
The following technology plan lists potential technologies to be used in the creation of our application and a personal experience rating for each technology.

| Technology | Experience Rating |
|------------|-------------------|
| Mobile App Technologies | |
| iOS | None |
| Android | Tutorial |
| Cordova | Small Scale |
| Windows 10 Phone | None |
| Map Technologies | |
| Google Maps | Tutorial |
| Bing Maps | None |
| Open Layers Maps | None |
| Open Street Maps | None |
| Application and Web Development | |
| Java | Extensive |
| Swift | None |
| HTML 5 | Moderate |
| Javascript | Moderate |
| jQuery Mobile | Small Scale |
| Bootstrap Framework | Tutorial |
| Iconic Framework | None |
| Web Server Scripting | |
| PHP | Small Scale |
| Microsoft ASP.NET | Extensive |

## Risk Analysis

<div name="technical-risk-by-business-goal">
 <h3>Technical Risk by Business Goal</h3>
</div>

The following technical risks and business goals have been identified and prioritized.

| ID | Technical Risk | Business-Market | Business-Users | Business-Value |
|----|----------------|-----------------|----------------|----------------|
| Tech-R-1 | Limited experience developing mobile apps. | - | H | H |
| Tech-R-2 | No experience accessing the GPS in a mobile app | - | H | H |
| Tech-R-3 | Implementing offline map and GPS access is not the normal mode of map operation for a mobile app | M | H | H |
| Tech-R-4 | Tools needed to conduct the project such as the IDE, Visual Paradigm, Bitbucket, Markdown, and Git are new | M | H | H |
| Tech-R-5 | Time for the developer to work on the project is limited due to the demands of their class schedule | M | - | - |
| Tech-R-6 | Inadequate testing does not cover requirements | L | - | - |
| Tech-R-7 | The app is susceptible to cross-site scripting attacks | M | - | - |

<div name="risk-mitigation-plan">
  <h3>Risk Mitigation Plan</h3>
</div>

The following risk mitigation plan will help us to address and mitigate these risks to the extent possible.
 
| ID | Risk | Mitigation |
|----|------|------------|
| Tech-R-1 | Limited experience developing mobile apps. | Schedule for and work through online tutorials |
| Tech-R-2 | No experience accessing the GPS in a mobile app | Schedule for and work through online tutorials |
| Tech-R-3 | Implementing offline map and GPS access is not the normal mode of map operation for a mobile app | Search for information and tutorials on offline map access |
| Tech-R-4 | Tools needed to conduct the project such as the IDE, Visual Paradigm, Bitbucket, Markdown, and Git are new | Schedule time in the schedule to learn these tools using tutorials found online |
| Tech-R-5 | Time for the developer to work on the project is limited due to the demands of their class schedule | Explicitly use a calendar to plan daily schedules allocating spcific time periods to work on the project |
| Tech-R-6 | Inadequate testing does not cover requirements | Utilize automated testing tools. Make testing a priority activity |
| Tech-R-7 | The app is susceptible to cross-site scripting attacks | Follow the OWASP guidelines for preventing cross-scripting attacks and the OWASP testing protocol |
