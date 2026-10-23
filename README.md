
# QoDe — AI-Powered Road Safety

**TEKNOFEST 2026 Finalist | 5G & AI Smart Road Safety Competition**

QoDe is an AI-powered road safety system developed for TEKNOFEST 2026. It analyzes roadside camera footage to identify vehicles, recognize license plates, and detect driver behaviors and potential traffic safety violations.

The project combines computer vision, deep learning, backend services, and a Kotlin Android application.

## Key Features

- **Vehicle Analysis:** Detects vehicles and identifies their type, color, and license plate.
- **Driver Monitoring:** Analyzes driver actions such as phone usage, drinking, and signs of distraction.
- **Video Processing:** Combines object detection, image classification, OCR, and temporal filtering.
- **Android Application:** Streams video from a server and communicates with the AI backend to request video analysis.
- **Structured Results:** Produces timestamped detection results with confidence scores in a competition-compatible JSON format.

## Technology Stack

| Component | Technologies |
|---|---|
| Computer Vision | YOLO11, OpenCV |
| Deep Learning | PyTorch, EfficientNet |
| OCR | EasyOCR |
| Backend | Python, HTTP APIs |
| Mobile | Kotlin, Android |
| Deployment | Docker |

## System Overview

The system consists of three main components:

1. **Video Processing:** Camera footage is processed using detection and classification models to extract vehicle information and driver behavior.
2. **AI Backend:** Model inference results are organized, validated, and exposed through backend services.
3. **Android Application:** Users can view server-provided video streams and send analysis requests to the AI backend.

The computer vision pipeline combines YOLO-based detection, EfficientNet classifiers, EasyOCR, and temporal post-processing.

## Development and Evaluation

The project includes dataset preprocessing, model training, inference, and evaluation tools. Supporting datasets include State Farm Distracted Driver, DMD, and DriverSVT.

Detection quality depends on video resolution, environmental conditions, and the available training data. Some competition-specific integrations require external credentials or infrastructure.

## Competition

Developed as a team project for the **TEKNOFEST 2026 5G and Artificial Intelligence Smart Road Safety Competition**, reaching the finalist stage.

## Documentation

Detailed implementation information, competition specifications, training scripts, and evaluation resources are available in the repository's `docs/` directory and source code.
