# Collision Prevention System for Satellites using Space Debris Management

## Overview

This project implements a Collision Prevention System for satellites, which predicts potential collisions with space debris and provides predictive trajectory analysis. The system is designed with robust software engineering principles, ensuring scalability, maintainability, and clear division of tasks as outlined in the Work Breakdown Structure (WBS) and Use Case Diagram.

## Project Structure

### Work Breakdown Structure (WBS)

The project is structured into distinct modules, each responsible for a specific aspect of the system:

1. **Data Simulation and Preprocessing**
   - Simulate satellite trajectories for both training and testing.
   - Preprocess the data to ensure compatibility with the machine learning models.

2. **Collision Risk Assessment**
   - Implement a classifier to assess the risk of collision based on satellite trajectory data.
   - Use features like `PERIAPSIS` and `APOAPSIS` to determine high-risk scenarios.

3. **Trajectory Prediction**
   - Develop and train an LSTM model to predict future satellite positions based on historical trajectory data.
   - Provide predictive trajectories for both training and test scenarios.

4. **Evaluation and Visualization**
   - Evaluate model performance using standard metrics.
   - Visualize the predicted collision risk and trajectory paths.

### Use Case Diagram

![Use Case Diagram](https://github.com/rohan-mn/Collision-Prevention-System-for-Satellites-using-Space-Debris-Management/blob/831f390a22584ba0d6419ae0e14b7c7ffa58421c/Use%20case%20diagram.png)  
The use case diagram outlines the primary interactions between the user and the system:

1. **User Input**: The user provides initial satellite trajectory data.
2. **Collision Risk Assessment**: The system processes the data and provides a collision risk prediction.
3. **Predictive Trajectory**: If a collision risk is detected, the system provides a predicted trajectory to avoid the collision.
4. **User Feedback**: The user can review the predictions and decide on corrective actions.

## Installation

To get started with the project, ensure you have the following dependencies installed:

- Python 3.x
- TensorFlow
- NumPy
- Pandas
- Scikit-learn

Install the required packages using:

```bash
pip install -r requirements.txt
