# Detecting Fake Vehicles in V2X Communication Networks

## Overview
This project addresses the threat of sensor spoofing in V2X (Vehicle-to-Everything) communication networks. Sensor spoofing enables attackers to inject false data into a vehicle’s communication system, potentially leading to:

- Traffic accidents  
- Disruption of vehicle coordination  
- Security breaches in autonomous driving environments

To mitigate this, a machine learning-based solution using a Random Forest Classifier is implemented to detect fake or anomalous vehicles based on behavioral and signal-based features.

## Problem Statement: Sensor Spoofing in V2X

Sensor spoofing attacks simulate legitimate vehicle behavior by manipulating transmitted data. Key types of spoofing include:

- GPS Spoofing: False location data is transmitted to misrepresent a vehicle’s position.  
- Speed and Acceleration Tampering: Abnormal speed or acceleration values are reported.  
- Communication Interference: The attacker floods the network with false messages or uncooperative nodes.

These attacks compromise safety, traffic flow, and data integrity in V2X-enabled networks.

## Proposed Solution

The system uses a Random Forest Classifier to differentiate between real and fake vehicles. The classifier is trained on a labeled dataset comprising both real and spoofed sensor data.

### Key Features for Detection

- V2X communication patterns (e.g., message frequency, error rate)
- GPS data consistency and spatial coherence
- Signal strength and transmission reliability
- Vehicle behavior metrics (e.g., speed, acceleration)

## System Workflow

1. **Data Collection**  
   Data is gathered from simulated V2X environments including both legitimate and spoofed vehicle data.

2. **Feature Engineering**  
   Relevant features are extracted from raw logs such as GPS stability, signal patterns, and speed consistency.

3. **Model Training**  
   A Random Forest Classifier is trained on the labeled dataset to learn patterns of legitimate vs. spoofed data.

4. **Detection & Prediction**  
   Incoming data from vehicles is classified as either "Real" or "Fake" based on learned behavior and signal traits.

## Use Cases

- Intrusion detection systems in smart transportation networks  
- Security assurance for autonomous vehicle communication  
- Research on cyber-physical security in vehicular networks

