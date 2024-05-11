
# Object Detection using YOLO-NAS-L

This project demonstrates how to perform object detection using the YOLO-NAS-L architecture. It allows detecting persons in images, videos, or streaming sources.

## Installation

1. Clone this repository to your local machine:

```bash
git clone https://github.com/yourusername/object-detection.git
```

2. Install the required dependencies:

```bash
pip install -r requirements.txt
```

## Usage

### Using the Object Detector class

```python
import cv2
import numpy as np
from object_detector import ObjectDetector
from super_gradients.common.object_names import Models
from super_gradients.training import models

# Load the YOLO-NAS-L model
model = models.get(Models.YOLO_NAS_L, pretrained_weights="coco")

# Instantiate the ObjectDetector with the loaded model
detector = ObjectDetector(model)

# Path to the input video
input_video_path = "input_video.mp4"

# Path to save the output video with predictions
output_video_path = "output_video.mp4"

# Number of frames to process (optional)
max_frames = 500

# Confidence threshold for object detection (optional)
confidence_threshold = 0.2

# Call the detect_objects method to process the video and save the output video with predictions
detector.detect_objects(input_video_path, output_video_path, max_frames=max_frames, confidence_threshold=confidence_threshold)
```

### Supported Input Types

The Object Detector class supports the following input types:

- Video files: `.mp4`, `.avi`, etc.
- Image files: `.jpg`, `.jpeg`, `.png`, `.bmp`
- Streaming sources: HTTP/HTTPS links to video streams

### Output

The `detect_objects` method saves the output video with bounding boxes and confidence scores drawn around detected persons. Additionally, it prints the path to the saved video.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
