Suspicious Activity Detection

## Project Overview
The Suspicious Activity Detection project aims to identify potentially suspicious activities using machine learning techniques. This system leverages advanced algorithms to analyze video footage and detect unusual behaviors that may indicate suspicious actions.

## Installation
To set up the project, follow these steps:

1. Clone the repository:
   git clone https://github.com/yourusername/Suspicious_Activity_Detection.git

2. Navigate to the project directory:
   cd Suspicious_Activity_Detection

3. Install the required dependencies:
   pip install -r requirements.txt

## Usage
To run the project, use the following commands:

 1. Training the Model:
  python train.py --data data.yaml --cfg yolov5s.yaml --weights yolov5s.pt --epochs 100

 2. Validating the Model:
  python val.py --data data.yaml --weights yolov5s.pt

 3. Making Predictions:
  python predict.py --source video.mp4 --weights yolov5s.pt --conf 0.25 --name results

Replace `video.mp4` with your input video file and adjust the confidence threshold (`--conf`) as needed.

## Directory Structure
The repository is organized as follows:

Suspicious_Activity_Detection/
├── figure/                  # Directory for figures and images
├── ultralytics/             # Contains YOLOv5 implementation
├── .gitattributes           # Git attributes file
├── .gitignore               # Git ignore file
├── predict.py               # Script for making predictions
├── requirements.txt         # List of required packages
├── setup.cfg                # Configuration file for the project
├── setup.py                 # Setup script for installing the package
├── train.py                 # Script for training the model
└── val.py                   # Script for validating the model

## Contributors
- Devashish Juyal - Initial work
- Shreyash Methi - Initial work

## License
This project is licensed under the MIT License - see the LICENSE file for details.
