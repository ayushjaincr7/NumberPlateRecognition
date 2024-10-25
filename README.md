# NumberPlateRecognition
<a href="https://drive.google.com/file/d/10KBP8q2HxNHWr6OQYy_rj59q4jeq4Ojj/view?usp=sharing">Vidoes Source</a>
--------> <a href="https://drive.google.com/file/d/1JWKzybhnL0p5_jXtvOrumdejhT_jGyA8/view?usp=drive_link">Videos Output</a>


<br>
1.	YOLOv8 for Vehicle Detection:
	.	Purpose: To detect cars and other vehicles in each frame of the video.
	•	Pre-trained Model: You’re using YOLOv8 (e.g., yolov8n.pt) trained on the COCO dataset, focusing on vehicle classes like cars, buses, and trucks.
2.	YOLOv8 for License Plate Detection:
	•	Purpose: To detect license plates on the detected vehicles.
	•	Custom Model: A YOLOv8 model (best.pt) fine-tuned for detecting license plates, possibly trained on a custom dataset.
3.	SORT Algorithm:
	•	Purpose: To track detected vehicles across video frames. This maintains consistency in identifying and tracking cars even when the vehicle moves or the frame changes.
4.	EasyOCR for Text Recognition:
	•	Purpose: To extract the license plate number from the cropped image of the license plate.
	•	Process:
	•	Convert the detected license plate image to grayscale and apply thresholding for better clarity.
	•	Use EasyOCR to read the license plate text from the processed image.
