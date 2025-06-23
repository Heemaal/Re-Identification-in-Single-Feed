# Re-Identification-in-Single-Feed
This project demonstrates real-time player detection and re-identification in a 15-second sports video using a custom YOLOv5 object detection model. The key objective is to consistently assign unique IDs to players — even when they leave and re-enter the frame — simulating a real-time tracking system.

# Player Tracking and Re-Identification in Sports Video

This project demonstrates real-time player detection and re-identification in a short 15-second sports video. The objective is to detect players using a YOLOv5 object detection model and assign consistent player IDs, even when players leave and re-enter the frame. This simulates real-time tracking for sports analytics applications.

## Problem Statement

**Objective:**
Given a 15-second sports video clip (`15sec_input_720p.mp4`), detect all players using a custom-trained YOLO model, assign unique IDs, and maintain those IDs when players reappear later in the frame.

## Features

- Object detection using YOLOv5 trained for players and ball
- Real-time player re-identification with consistent ID assignment
- Frame-by-frame video annotation with bounding boxes and player IDs
- Final output video with all detections and tracking information

## Tech Stack

- **Python**: Used as the primary programming language.
- **YOLOv5 (Ultralytics)**: For object detection of players and the ball.
- **OpenCV**: To handle video input/output and annotate frames.
- **DeepSORT**: Used for multi-object tracking and re-identification of players.
- **Google Colab**: For running the entire pipeline in a cloud-based environment.

## File Structure

- `15sec_input_720p.mp4`: Input sports video used for detection and tracking.
- `custom_model.pt`: YOLOv5 model trained to detect players and the ball.
- `output_detected.mp4`: Final video output with tracked player IDs.
- `track_players.ipynb`: Google Colab notebook with full code implementation.

## How to Run (in Google Colab)

1. Open the `Real-time player tracker` notebook .
2. Upload the following files when prompted:
   - `15sec_input_720p.mp4`
   - `custom_model.pt`
3. Run all cells in the notebook to:
   - Load the object detection model
   - Perform frame-by-frame detection and tracking
   - Generate and download the final output video

## Sample Output

*A frame from the output video showing bounding boxes and consistent player IDs.*

![image](https://github.com/user-attachments/assets/8e84a995-90c3-4f10-8aca-10d16bb5f347)


## Future Enhancements

- Player speed and movement analysis
- Ball trajectory tracking
- Event detection (passes, goals, fouls)
- Team color-based re-identification for better accuracy

## Author

**Heemaal Jaglan**  
Focused on AI, Machine Learning, and Data Analytics  
GitHub: https://github.com/Heemaal
LinkedIn: https://www.linkedin.com/in/heemaal-jaglan-144bb225b/
## License

This project is for educational and demonstration purposes only. No commercial use is intended for the dataset or trained model.
