# Dataset

This folder contains the datasets used in the research project **"Multi-Task Transformer for Yoga Pose Recognition and Injury Risk Assessment."**

## Processed Dataset

The processed dataset consists of MediaPipe Pose landmark keypoints extracted from the original yoga videos.

**Contents:**
- `yoga_video_keypoints.csv` (compressed as `.zip`)

**Download:**
https://drive.google.com/drive/folders/143OM0j38K5uGND4MR4qN85LXLBmpMsCh?usp=sharing

**Description:**
- Contains the extracted 3D pose landmarks (`x`, `y`, `z`) for each video frame.
- Used for biomechanical feature extraction, sequence generation, model training, and evaluation.
- The CSV is provided as a ZIP archive due to GitHub file size limitations.

---

## Raw Video Dataset

The original yoga videos used to generate the processed dataset are available below.

**Download:**
https://drive.google.com/drive/folders/1tCioHTCCwzpAbWRgOlNwV3wWKweACANL?usp=sharing

**Description:**
- Original yoga posture videos.
- Used as the input for MediaPipe Pose landmark extraction.
- Served as the source data for generating the `yoga_video_keypoints.csv` dataset.

---

## Data Processing Pipeline

```
Raw Yoga Videos
        │
        ▼
MediaPipe Pose Landmark Extraction
        │
        ▼
yoga_video_keypoints.csv
        │
        ▼
Feature Engineering
(Biomechanical Features + Landmark Sequences)
        │
        ▼
Multi-Task Transformer
(Pose Recognition + Injury Risk Assessment)
```

## Notes

- The processed dataset was generated directly from the raw yoga videos using MediaPipe Pose.
- Both datasets are hosted on Google Drive because they exceed GitHub's recommended file size limits.
- The preprocessing, feature engineering, training, and evaluation pipeline are fully documented in the training notebook located in the `notebooks/` directory.
