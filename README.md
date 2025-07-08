# Multiperson Pose Estimation using YOLOv8 & Mediapipe 🤖

This project combines YOLOv8 (for people detection) and Mediapipe (for pose estimation) to detect and visualize the poses of **multiple people** in a video.

---

## 🎯 Project Overview

Since **Mediapipe Pose** only supports **single-person detection**, this project:
- Uses **YOLOv8** to detect multiple people
- Crops each detected person out of the frame
- Applies **Mediapipe Pose** on each person
- Reconstructs the annotated full-frame video with all pose estimations

---
📁 Project Structure and File Purpose
File	Description
| File                                                                                                                          | Description                                                                                            |
| ----------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------ |
| [`YOLOv8_&_Mediapipe.ipynb`](https://github.com/moaaz12-web/Multiperson-pose-estimation/blob/main/YOLOv8_%26_Mediapipe.ipynb) | 💡 **Main notebook**. Runs the full pipeline: detection → cropping → pose estimation → output video.   |
| `download (4).mp4`                                                                                                            | 🎥 **Input video** to test the detection and pose tracking system. You can replace this with your own. |
| `labeled_client_sent_4_ppl.mp4`                                                                                               | 🧍‍♂️ **Output video** created by the notebook, showing poses drawn over each detected person.         |
| `README.md`                                                                                                                   | 📘 Project instructions, overview, and setup guide (this file).                                        |

## 🧰 Requirements

Install dependencies:

```bash
pip install mediapipe ultralytics opencv-python numpy pandas
