UCS Ontology - Urban Cycling Safety
Overview
The Urban Cycling Safety (UCS) ontology is designed to represent knowledge related to bicycle riding scenarios in urban environments. This ontology fills the gap left by existing ontologies in the Automated Driving (AD) domain, which do not fully cover cycling safety. The UCS ontology models urban cycling safety by considering various road networks, traffic participants, environmental conditions, and dynamic context elements that affect cycling behavior and safety.

Structure
The UCS ontology comprises four core interrelated classes:

Scenario
Scene
Situation
Dynamic Context Elements
These classes maintain hierarchical relationships to model real-world urban cycling scenarios, breaking down high-level scenarios into specific scenes and situations.

Key Features of UCS Ontology
Scene Class: This class is divided into five subclasses, each representing a different layer of the urban cycling scene:

Road Network Layer: Models the road topology, such as lanes, junctions, and intersections.
Road Infrastructure Layer: Captures physical elements like traffic signs, lights, pedestrian crossings, etc.
Traffic Participant Layer: Includes entities such as cyclists, pedestrians, and vehicles.
Environment Layer: Models environmental factors like rainfall, temperature, and wind.
Sensor Layer: Represents sensors that observe and gather data about the scene.
Dynamic Context Element Class: This class represents context-related elements like person, environment, vehicle, and road. Each context dimension is modeled with specific subclasses, such as "Traffic Condition" under Road Context with subclasses like "High Traffic," "Moderate Traffic," and "Low Traffic."

Situation Class: Contains six primary categories to represent different types of situations:

Vehicle-related Situations (Bicycle-related, Four-Wheeled Vehicle-related)
Pedestrian-related Situations
Road-related Situations
Traffic Participant-related Situations
Weather-related Situations
Emergency Response Situations
Event Class: Defines events originating from entities or external triggers. These events, like vehicle door opening or pedestrian crossing, drive situation state transitions.

Relationships and Object Properties
The ontology defines multiple relationships (object properties) to capture the interactions among the different layers and entities, including:

isInstalledOn: Links sensors to traffic participants, infrastructure, and environmental elements.
observes: Links sensors to dynamic context elements like speed, location, and traffic conditions.
hasState: Connects traffic participants to their respective states (e.g., "Riding," "Stopping").
We also extend existing ontologies, such as GeoSPARQL for spatial relationships and Time Ontology in OWL for temporal reasoning.

Use Case
The UCS ontology enables reasoning about various urban cycling safety situations. It can infer hazard situations based on contextual conditions such as traffic, road conditions, and weather, and help in evaluating potential risks to cyclists. For example:

Obstacle Ahead Situation: If a bicycle is approaching a stationary vehicle, the ontology infers a potential hazard.
Dooring Hazard: If a bicycle is near a parked vehicle with an open door, a "Dooring Hazard" situation is inferred.
Development Tools
The UCS ontology was developed using Protégé (Version 5.5.0).
The ontology incorporates semantic sensor data from SSN Ontology and external environmental and temporal ontologies.
Spatial and temporal relationships are modeled using GeoSPARQL and Time Ontology in OWL.
Future Work
This ontology is continually evolving, and future updates will focus on extending the domain coverage, enhancing reasoning capabilities, and integrating new data sources, such as real-time sensor data.

License
The UCS ontology is open-source and available for non-commercial use. Contributions and improvements are welcome through GitHub.

Note: This file provides an overview of the ontology’s structure, its components, and how it can be used to model urban cycling safety. For more detailed queries and examples, please refer to the ontology file and documentation.
