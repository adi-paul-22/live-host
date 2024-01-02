# Centralized Camera Location and Surveillance System

## Introduction

This application serves as a robust centralized surveillance system designed to manage and monitor CCTV cameras efficiently. The system employs a server infrastructure to receive, process, and analyze live camera feeds using advanced AI techniques to detect potential threats. Geo-tagging of each camera based on latitude and longitude facilitates location tracking, and a map visualization enhances the overall coverage overview.

## Key Features

### Centralized Server Infrastructure

- Manages the reception and processing of live camera feeds.
- Utilizes computer vision techniques to analyze video streams.
- Extracts essential metadata, such as location and status, for each camera.

### Hierarchical Unique ID System

- Assigns a unique identifier to each camera.
- Implements a hierarchical structure for efficient camera identification.

### Geo-tagging

- Tags cameras with latitude and longitude information.
- Enables visualization of camera locations on an interactive map.

### User Registration and Camera Authentication

- Requires user registration for system access.
- Implements secure authentication using Kerberos.
- Associates cameras with owners' accounts for personalized access.

### AI-powered Object and Facial Recognition

- Integrates YOLOv9 object detection model for threat identification.
- Utilizes facial recognition to identify unauthorized individuals.
- Displays bounding boxes to indicate AI detections.

### Alerting Mechanisms via MQTT

- Sends alerts to local authorities upon detecting threats.
- Utilizes MQTT for efficient and real-time alert dissemination.

## Architecture

### Server Infrastructure

- Receives and processes live camera feeds.
- Extracts metadata, including location and status, for each camera.
- Interfaces for camera registration, authentication, and health monitoring.
- Integration with AI models for object and facial detection.

### Camera Metadata

- Maintains a comprehensive database for each camera.
- Includes hierarchical location ID, owner information, health status, and more.
- Streaming resolution configuration for optimal video quality.

### Map Visualization

- Visualizes all cameras on an interactive map for each district.
- Facilitates a comprehensive overview of the surveillance area.
- Aids in identifying potential blind spots.

### User Authentication

- Requires user registration with verification documents.
- Cameras are securely assigned to owners' accounts.
- Implements Kerberos for secure and reliable authentication.

### AI and Alerting

- YOLOv9 model identifies threats in video frames.
- Facial recognition enhances security by identifying unauthorized individuals.
- Bounding boxes visually indicate the location of AI detections.
- Alerts are sent to local authorities in real-time via MQTT.
