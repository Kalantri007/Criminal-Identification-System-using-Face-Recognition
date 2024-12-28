# Criminal Identification System 

This repository contains the implementation of a **Criminal Identification System** using **2D Face Recognition**. The project leverages state-of-the-art image processing and machine learning techniques to detect and identify faces in real-time, aiding law enforcement agencies in criminal detection and surveillance.

---

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Motivation](#motivation)
- [Technology Stack](#technology-stack)
- [Software Engineering Practices](#software-engineering-practices)
- [Installation](#installation)
- [Usage](#usage)
- [Screenshots](#screenshots)
- [Testing](#testing)
- [Future Scope](#future-scope)
- [Contributors](#contributors)

---

## Overview

Face recognition is a powerful biometric method offering both **accuracy** and **low intrusiveness**. This system addresses limitations in traditional identification methods (e.g., fingerprints) by utilizing **CCTV footage** and **image processing algorithms** to match faces against a pre-trained database of criminal records. It provides a robust solution for real-time criminal detection at public and private locations.

---

## Features

- **Real-Time Face Detection and Recognition**: Identify individuals using a live camera feed.
- **Database Integration**: Store, update, and manage criminal records with ease.
- **Automated Alerts**: Sends notifications with details like location (latitude and longitude) upon detecting a match.
- **GUI Application**: User-friendly interface for system administrators and law enforcement officers.
- **Adaptability**: Works under varied lighting and disguise conditions.

---

## Motivation

With the advent of **CCTV systems** and the increasing need for automated surveillance, the current manual methods of identifying suspects are time-consuming and error-prone. This system was built to:
- Enhance **criminal identification efficiency**.
- Reduce dependency on manual identification techniques.
- Leverage advancements in **AI and machine learning** for social benefit.

---

## Technology Stack

- **Programming Language**: Python (3.7+)
- **Libraries & Tools**:
  - [OpenCV](https://opencv.org/) - For image processing.
  - [MySQL](https://www.mysql.com/) - Backend database.
  - [Tkinter](https://docs.python.org/3/library/tkinter.html) - GUI development.
- **Algorithms**:
  - Haar Cascade Classifier for face detection.
  - Custom-trained Convolutional Neural Networks (CNN) for face recognition.
- **Other Tools**:
  - SMTP for email notifications.
  - Python IDLE for development.

---

## Software Engineering Practices

This project adheres to modern **Software Engineering** practices to ensure maintainability, scalability, and reliability. Below are some key practices applied:

### Development Methodology
- **SDLC Model**: The project followed the **Waterfall Model**, which provided a structured, phase-wise approach to development, including:
  1. Requirement Gathering
  2. System Design
  3. Implementation
  4. Testing
  5. Deployment
  6. Maintenance

### Design Patterns
- **Modular Design**: Each feature (e.g., face detection, email alerts) is implemented as a separate module to ensure loose coupling and high cohesion.
- **MVC Architecture**: The system is designed with a clear separation of concerns:
  - **Model**: MySQL database.
  - **View**: Tkinter-based GUI.
  - **Controller**: Python scripts managing logic and interactions.

### Code Quality
- **PEP 8 Compliance**: The Python codebase adheres to PEP 8 style guidelines.
- **Version Control**: The project uses Git for tracking changes and collaborating among team members.

### Testing Strategy
- **Test-Driven Development (TDD)**: Unit tests were written alongside feature implementation to ensure early detection of bugs.
- **Automated Testing**: Scripts were created to automate regression and functional testing.

### Security Considerations
- **Data Validation**: Input fields validate user data to prevent SQL injection and invalid entries.
- **Secure Communication**: SMTP settings for email alerts use secure connections (TLS/SSL).

### Tools Used
- **GitHub Issues**: For bug tracking and feature requests.
- **Gantt Charts**: Used for project scheduling and progress tracking.
- **Documentation**: Comprehensive project documentation, including design diagrams (UML), was maintained.

---

## Usage

### Launch the GUI Application
To start the application, launch the GUI from the main executable or script. The application will provide the following features:

1. **Add Police Station**: Register police stations with their contact details.
2. **Add Criminal Record**: Add new criminal data with images for training the model.
3. **Train Model**: Train the recognition model with updated criminal records.
4. **Live Camera Feed**: Activate the camera for real-time face recognition.
5. **Notifications**: Receive alerts for recognized individuals.

## Testing

The application was tested using the following methods:

- **Unit Testing**: Each module, such as face detection and database integration, was tested individually to ensure functionality.
- **Integration Testing**: End-to-end functionality testing was performed to ensure that all modules work together seamlessly.
- **Performance Testing**: The system has been optimized for performance, with a minimum requirement of 8GB of RAM.
- **Security Testing**: Secure handling of sensitive data, such as criminal records, has been thoroughly verified.

## Future Scope

- Enhance face recognition accuracy with advanced techniques such as **Principal Component Analysis (PCA)** and **Fisher's Linear Discriminant Analysis (FLDA)**.
- Extend support for **video-based recognition**, accommodating varying poses and lighting conditions.
- Integrate with **cloud-based databases** for scalable storage and processing.
- Develop a **mobile application** for field officers to use on the go.
