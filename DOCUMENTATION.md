PROJECT REPORT: SMAART CAMPUS NAVIGATOR WEB APP
1. Introduction
1.1 Purpose
The Pragati Campus Navigator is an interactive, web-based mapping application designed to streamline navigation within the college premises. It provides a digital alternative to static physical signboards, offering real-time location tracking and pathfinding.

1.2 Scope
This application is intended for students, faculty, and visitors. It covers all major academic blocks (Main, ECE, MECH, AIML), amenities (Canteen, Library), and residential areas (Hostels).

2. System Requirements
2.1 Hardware Requirements
Processor: Dual-core 2.0 GHz or higher.

RAM: 2GB minimum (4GB recommended).

Device: Smartphone with GPS or Laptop with Wi-Fi.

2.2 Software Requirements
Operating System: Windows, macOS, Android, or iOS.

Web Browser: Google Chrome, Safari, or Mozilla Firefox.

Library: Leaflet.js (Open Source).

Map Data: OpenStreetMap API.

3. System Architecture
The application follows a Client-Side Architecture.

User Interface (UI): Built with HTML5 and CSS3 for a responsive "App-like" feel.

Mapping Engine: Leaflet.js handles the rendering of map tiles and markers.

Coordinate System: Uses a custom JSON-style array of Latitude and Longitude coordinates specific to the Pragati Campus.

4. Detailed Design & Modules
4.1 Dashboard Module
The landing page features a maroon-themed gradient UI with four primary functional cards:

Map: Transitions the user to the interactive campus view.

Search: Automatically focuses the search bar for quick navigation.

Directions: Opens the route-planning interface.

Feedback: A simple interaction layer to collect user experience data.

4.2 Navigation & Pathfinding
The pathfinding logic uses the Polyline Method. When a user selects a "From" and "To" location, the system fetches the coordinates from the internal database and draws a blue vector line on the map.

4.3 Geolocation Module
The app utilizes the HTML5 Geolocation API.

It requests the user's current GPS coordinates.

It renders a blue circle marker (userMarker) to show exactly where the student is standing on campus.

5. Data Dictionary
The application stores the following key landmarks:

Landmark	Latitude	Longitude
Library	17.0836	82.0536
Main Block	17.0836	82.0534
Mechanical Block	17.0836	82.0538
Canteen	17.0833	82.0536
AIML Block	17.0839	82.0538
6. Testing & Validation
To ensure the application works correctly, the following tests were conducted:

Test Case	Action	Expected Result	Status
Initialization	Open App	Dashboard loads with maroon theme.	Pass
Search Function	Type "Library"	Map zooms into Library coordinates.	Pass
Pathfinding	Library to Canteen	A blue line appears between the two.	Pass
Geolocation	Click "Locate"	Blue dot appears at current user position.	Pass
7. Conclusion
The Pragati Campus Navigator successfully demonstrates how open-source mapping technologies can be customized for localized environments. The project is lightweight, requires no installation, and provides an essential service for modern campus management.

8. References
Leaflet.js Documentation: leafletjs.com

OpenStreetMap Wiki: openstreetmap.org

MDN Web Docs: Geolocation API.
9. Project Team & Contributions
Name,Role,Responsibilities & Contributions
K.Surekha,Lead Developer,"Responsible for core JavaScript logic, Leaflet.js integration, and coordinate mapping."
T,Suvarna,UI/UX Designer,"Focused on CSS styling, the maroon dashboard interface, and ensuring mobile responsiveness."
P.Akshaya,Research & QA,"Handled GPS data collection for campus landmarks, project documentation, and system testing."
