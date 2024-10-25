# NumberPlateRecognition


This project aims to automatically detect vehicles and recognize their license plates from video frames using advanced computer vision techniques.

## 1. YOLOv8 for Vehicle Detection
- **Purpose**: Detect cars and other vehicles in each frame of the video.
- **Pre-trained Model**: YOLOv8 (`yolov8n.pt`), trained on the COCO dataset to detect vehicle classes like cars, buses, and trucks.

## 2. YOLOv8 for License Plate Detection
- **Purpose**: Identify license plates within the detected vehicles' bounding boxes.
- **Custom Model**: A fine-tuned YOLOv8 model (`best.pt`) specifically trained on a custom dataset for detecting license plates.

## 3. SORT Algorithm
- **Purpose**: Track detected vehicles across video frames. This ensures consistency in identifying and tracking cars even as they move or the frame changes.

## 4. EasyOCR for Text Recognition
- **Purpose**: Extract the license plate number from the cropped image of the detected license plate.
- **Process**:
  1. Convert the detected license plate image to grayscale.
  2. Apply thresholding to improve clarity for OCR.
  3. Use EasyOCR to read and extract text from the processed license plate image.
 

<a href="https://drive.google.com/file/d/10KBP8q2HxNHWr6OQYy_rj59q4jeq4Ojj/view?usp=sharing">Vidoes Source</a>
--------> <a href="https://drive.google.com/file/d/1JWKzybhnL0p5_jXtvOrumdejhT_jGyA8/view?usp=drive_link">Videos Output</a>

