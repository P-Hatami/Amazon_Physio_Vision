# Physio-Vision: Fire TV Aged-Care Assistant

Physio-Vision is a lightweight, computer-vision-powered simulation built for the Amazon Fire TV ecosystem. It transforms a standard smart TV setup into a proactive aged-care monitoring system without requiring expensive external hardware.

## Key Features
*   **Real-time Fall Detection:** Utilizes OpenCV contour analysis and aspect-ratio tracking to instantly detect if an elderly individual has fallen.
*   **Recovery Detection:** Automatically switches off alarms and updates status if the individual stands back up safely.
*   **Automated Event Logging:** Generates a `physio_vision_logs.csv` file, timestamping critical events (falls and recoveries) for medical professionals or family members to review.
*   **Calibrated UI Grid:** Simulates a professional monitoring dashboard directly on the Fire TV interface.

## How to Run (Simulator)
1. Clone the repository.
2. Install the requirements: `pip install opencv-python numpy`
3. Run the application: `python physio_vision.py`
4. Stand in front of the webcam to see the tracking bounding box. Simulate a fall by dropping below the horizontal threshold to trigger the visual and audio alarm.
