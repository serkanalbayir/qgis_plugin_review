# qgis_plugin_review

A work from my undergraduate education

[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/Y9vXfndP)

# HACETTEPE UNIVERSITY GEOMATIC ENGINEERING GMT456 FINAL PROJECT

**Student:** Serkan Albayır  
**Student ID:** 21967282


# Closest Points QGIS Plugin

This QGIS plugin, named "Closest Points," is designed to find the nearest points between two vector layers. It offers two main algorithms:

## 1. find_closest_point Algorithm

- This algorithm identifies the nearest point in the second layer for each feature in the first layer.
- The result is a new layer containing the feature ID and distance for each feature's nearest point.

## 2. find_all_closest_points Algorithm

- This algorithm discovers the nearest points between features in both layers.
- For each feature, it identifies the nearest point among all features in the other layer.
- The result layer includes the feature ID, distance, and geometry of the nearest point for each feature.

## Usage

To access the plugin, follow these steps:

1. **Installation:**
   - Install the plugin through the QGIS Plugin Manager.

2. **Menu/Toolbox Access:**
   - Access the plugin through the QGIS menu under "Closest Points" or via the Processing Toolbox.
  
   ![image](https://github.com/GMT-456-GIS-Programming/final-project-serkanalbayir/assets/115184884/e554ecd9-11eb-42a4-b37c-fe97b04611f3)

3. **Algorithm Options:**
   - Two algorithm options are available: `find_closest_point` and `find_all_closest_points`.

4. **find_closest_point:**
   - Select this option to find the nearest points for each feature in the first layer from the second layer.
   - Choose two vector layers as input.

5. **find_all_closest_points:**
   - Select this option to find the nearest points between features in both layers.
   - Choose two vector layers as input.

6. **Result:**
   - Once the process is complete, the results are added as a new layer.

## Code Evaluation

### 1. Overall Structure

The code follows a modular structure:

- Each algorithm (`find_closest_point` and `find_all_closest_points`) is implemented in separate files.
- Algorithms have their own classes and methods, enhancing code organization.

### 2. Language Support

- The code includes language files for localization, allowing the user interface to be presented in different languages.

### 3. QGIS API

- Utilizes the QGIS API for parameter definitions, layer operations, and result processing.

### 4. GUI Management

- The `initGui`, `run`, and `unload` methods handle graphical interface operations for toolbar buttons, menu additions, and displaying the plugin window.

### 5. Processing Framework Usage

- Algorithms are integrated into the Processing Framework, enabling the definition and execution of geospatial processes within QGIS.

### 6. Error Handling

- Includes control mechanisms for error situations and utilizes error messages to handle faulty conditions.


