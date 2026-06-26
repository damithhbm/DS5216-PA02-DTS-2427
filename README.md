# DS5216 Programming Assignment 02 - Player Tracking in Sports Videos

## Student Details
- Student ID: DST/24/27
- Module: DS5216 Artificial Intelligence
- Assignment: Programming Assignment 02

## Project Overview
This project implements a computer vision solution for detecting and tracking players in sports videos. A YOLO11-based object detection model was fine-tuned to detect players, and ByteTrack was used to track player movement across video frames. A YOLO pose estimation model was also used for the bonus keypoint detection task.

## Dataset
Sports video clips were collected from publicly available YouTube sources. Each clip was trimmed to 8 seconds and frames were extracted at 10 FPS.

Dataset video links are included in the notebook.

## Methodology
1. Collected 5-10 sports video clips from YouTube.
2. Trimmed each clip to 8 seconds.
3. Extracted video frames at 10 FPS.
4. Used a pretrained YOLO11 model to generate player labels.
5. Fine-tuned YOLO11 for player detection.
6. Used ByteTrack for player tracking.
7. Used YOLO Pose for keypoint detection.

## Model Performance

| Metric | Value |
|---|---:|
| Precision | 0.83899 |
| Recall | 0.78985 |
| mAP50 | 0.87562 |
| mAP50-95 | 0.71212 |

## Repository Structure

```text
notebook/       Jupyter notebook implementation
report/         Final assignment report
screenshots/    Output screenshots
inouts/        Dataset(links)
