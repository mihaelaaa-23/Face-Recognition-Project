# Face Recognition Attendance System

## Overview

This project implements a face recognition-based attendance system using Python, OpenCV, and the `face_recognition` library. It captures faces via a webcam and matches them against a pre-encoded list of known faces to record attendance automatically in a CSV file. Each recognized face is logged with their name, the date, and the time of recognition, ensuring accurate and timely attendance tracking.

## Project Structure

- **AttendanceProject.py**: Main script that captures video from a webcam, recognizes faces, and records attendance.
- **Basics.py**: Script demonstrating basic face recognition tasks including loading, encoding, and comparing face images.
- **ImagesAttendance/**: Directory containing images used for building the known face encodings.
- **Attendance.csv**: CSV file where attendance records are stored. New entries are added with name, date, and time for each recognized individual.
- **ImagesBasic/**: Directory containing test images for the basic face recognition demonstration.

## Setup

### Prerequisites

- Python 3.8+
- OpenCV
- face_recognition
- numpy

### Installation

1. Install Python dependencies:
   ```bash
   pip install numpy opencv-python face_recognition
   ```

2. Clone this repository:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```

3. Prepare the `ImagesAttendance` directory by placing images of individuals you want to recognize. Each image should be named as `<name>.<ext>` where `<name>` is the person's name.

4. Ensure you have a webcam connected to your computer for capturing video.

## Usage

### Recording Attendance
To start the attendance system, run the `AttendanceProject.py` script:
```bash
python AttendanceProject.py
```
This script activates the webcam, detects faces, and records the attendance of recognized individuals into `Attendance.csv`. For each recognized face, the system appends a new line with the individual's name, the current date, and time to the CSV file. It will continue running until manually stopped.

### Testing Face Recognition
To test face recognition, run the `Basics.py` script:
```bash
python Basics.py
```
This script will load predefined images from `ImagesBasic` and show the recognition result on the screen.

## Contributing
Contributions to this project are welcome. Please ensure you adhere to clean code standards and provide comments where necessary.

## Contact
For bugs, features, or questions, please open an issue in the GitHub repository for this project.