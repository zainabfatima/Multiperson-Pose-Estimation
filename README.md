# Multiperson-pose-estimation
## Multiperson pose estimation using YOLOv8 and Mediapipe


This notebook uses YOLOv8 for people detection and then utilizes mediapipe for pose estimation. The process works by first detecting all people in a video frame, and then sending all those detected persons, one by one, to Mediapipe for pose estimation. The resulting output is then overlayed on each frame, resulting in a video with multiperson pose estimation. Since mediapipe only does pose estimation for single person, therefore we utilized YOLOv8 as a preprocessing step to acheive multiperson pose estimation.
