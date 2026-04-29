📍 SMAART Campus Navigator Web App

1. Introduction

1.1 Purpose

The Pragati Campus Navigator is an interactive, web-based mapping application designed to streamline navigation within the college premises. It provides a digital alternative to static signboards by offering real-time location tracking and pathfinding.

1.2 Scope

This application is intended for: 

- Students
- Faculty
- Visitors

It covers:

- Academic blocks (Main, ECE, MECH, AIML)
- Amenities (Canteen, Library)
- Residential areas (Hostels)



2. System Requirements

2.1 Hardware Requirements

- Processor: Dual-core 2.0 GHz or higher
- RAM: 2GB minimum (4GB recommended)
- Device: Smartphone with GPS or Laptop with Wi-Fi

2.2 Software Requirements

- Operating System: Windows, macOS, Android, iOS
- Web Browser: Chrome, Safari, Firefox
- Library: Leaflet.js (Open Source)
- Map Data: OpenStreetMap API



3. System Architecture

The application follows a Client-Side Architecture:

- User Interface (UI): Built using HTML5 and CSS3 for a responsive, app-like experience
- Mapping Engine: Leaflet.js renders map tiles and markers
- Coordinate System: Custom JSON-based latitude and longitude dataset for campus



4. Detailed Design & Modules

4.1 Dashboard Module

The landing page includes a maroon-themed UI with four main features:

- Map: Opens the interactive campus map
- Search: Focuses the search bar for quick access
- Directions: Route planning interface
- Feedback: Collects user input

4.2 Navigation & Pathfinding

- Uses the Polyline Method
- Fetches coordinates from internal data
- Draws a blue route line between locations

4.3 Geolocation Module

- Uses HTML5 Geolocation API
- Detects user’s real-time position
- Displays a blue marker on the map

---

5. Data Dictionary

Landmark| Latitude| Longitude
Library| 17.0836| 82.0536
Main Block| 17.0836| 82.0534
Mechanical Block| 17.0836| 82.0538
Canteen| 17.0833| 82.0536
AIML Block| 17.0839| 82.0538



6. Testing & Validation

Test Case| Action| Expected Result| Status
Initialization| Open App| Dashboard loads with maroon theme| Pass
Search Function| Type "Library"| Map zooms into Library coordinates| Pass
Pathfinding| Library to Canteen| A blue line appears between the two| Pass
Geolocation| Click "Locate"| Blue dot appears at current user position| Pass



7. Conclusion

The Pragati Campus Navigator demonstrates how open-source mapping technologies can be adapted for localized environments.

- Lightweight and fast
- No installation required
- Improves campus accessibility and navigation



8. References

- Leaflet.js Documentation: https://leafletjs.com
- OpenStreetMap: https://www.openstreetmap.org
- MDN Web Docs (Geolocation API): https://developer.mozilla.org



9. Project Team & Contributions

Name| Role| Responsibilities & Contributions
K. Surekha| Lead Developer| Core JavaScript logic, Leaflet.js integration, coordinate mapping
T. Suvarna| UI/UX Designer| CSS styling, dashboard design, mobile responsiveness
P. Akshaya| Research & QA| GPS data collection, documentation, testing

