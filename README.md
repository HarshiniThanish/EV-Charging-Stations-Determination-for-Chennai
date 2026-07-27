EV Charging Assistant

The EV Charging Assistant is a mobile application built using Flutter to help electric vehicle users find the most suitable charging stations based on their current battery level and driving range. Instead of simply displaying nearby stations, the application identifies charging stations that the vehicle can actually reach, helping users avoid unnecessary detours and reducing range anxiety.

The application calculates the vehicle's available driving distance using the battery's State of Charge (SoC) and the vehicle's full-charge range. It first identifies nearby charging stations using the Haversine formula and then uses the OSRM API to calculate the actual road distance and estimated travel time. This ensures that the recommendations are practical and accurate.

Users can view charging stations on an interactive map, compare multiple stations based on distance, charging power, and travel time, and access a tabular view for easier analysis. The application also supports GPS-based location detection and manual location selection for testing purposes.

The project follows a modular architecture with separate components for location services, routing, recommendation logic, and data management. A local CSV dataset of EV charging stations is used, making the application lightweight and easy to deploy.

Features
Calculates the vehicle's reachable distance using battery State of Charge (SoC).
Recommends charging stations that are within the vehicle's driving range.
Uses the Haversine formula to identify nearby charging stations.
Calculates real-world road distance and travel time using the OSRM API.
Displays charging stations on an interactive OpenStreetMap interface.
Allows users to compare charging stations based on distance, charging power, and travel time.
Provides both map and table views for better visualization.
Supports GPS-based and manual location selection.
Uses a local dataset, making the application fast and lightweight.
Technologies Used
Flutter
Dart
OpenStreetMap
OSRM API
Geolocator
CSV Parser
LatLong2
Future Improvements
Real-time charging station availability
Live traffic-based route optimization
Charging cost estimation
User login and charging history
