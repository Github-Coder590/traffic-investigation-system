# Automated CCTV Traffic / Road-Incident Investigation System

A university DAA project exploring a video-analysis pipeline for traffic
investigation using vehicle detection, multi-object tracking, and trajectory
analysis.

## Pipeline

1. Stage 1 — Video sampling and frame indexing.
2. Stage 2 — Vehicle detection using a MIO-TCD-trained YOLO11n baseline.
3. Stage 3 — ByteTrack-based tracking of detections.
4. Stage 4 — Trajectory and image-plane motion-feature extraction.

## Important limitations

- Small and distant vehicles may be missed by the detector.
- Bounding boxes and predicted vehicle classes may be imperfect.
- Track fragmentation and gaps may affect motion estimates.
- Velocity and acceleration are measured in image-plane pixels, not calibrated
  real-world units.
- The existing results are not a ground-truth tracking-accuracy evaluation.

## Notebook

Open `traffic_investigation.ipynb` in GitHub, or use the notebook's
Open in Colab link when one is added.

## Reproducibility

The notebook may depend on files, models, dependencies, and outputs stored
separately in Google Drive. A fresh Colab runtime may require additional setup.

## Data and model files

Large videos, datasets, model weights, and generated outputs are not included
in this repository by default.
