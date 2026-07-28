# YogaSafe AI

YogaSafe AI is a deep learning system that detects yoga poses, assesses injury risk, and explains which body joints contribute to the prediction.

## Repository Structure

```
notebooks/
    Complete Google Colab notebooks

dataset/
    Extracted MediaPipe keypoints dataset

model/
    Pretrained model and saved artifacts

frontend/
    HTML user interface

screenshots/
    Images used in this README
```

## Included Files

- **Yoga_Posture_Assessment_AI_Implementation_Thesis.ipynb**
  - Complete training, preprocessing, evaluation, and model development notebook.

- **YogaSafe_Slim_Inference.ipynb**
  - Lightweight notebook for inference only.
  - Loads the trained model and predicts pose and injury risk.

- **yoga_video_keypoints.csv**
  - Extracted pose landmark dataset.
  - Allows training without repeating MediaPipe extraction.

- **YogaModel_SavedArtifacts.zip**
  - Trained model, scalers, encoders, and required artifacts.

- **frontend/**
  - HTML and CSS files for the web interface.

## Requirements

```
Python 3.11
PyTorch
MediaPipe
OpenCV
NumPy
Pandas
Scikit-Learn
FastAPI
Uvicorn
Joblib
```

Install with

```bash
pip install -r requirements.txt
```

## Running the Inference Notebook

1. Open **YogaSafe_Slim_Inference.ipynb**
2. Run all cells in order.
3. Upload a yoga video.
4. Receive:
   - Pose prediction
   - Injury risk prediction
   - Joint-level explanation

## Authors
- John Carlos Nico Reyes
- Rafael Benipayo
- Julia Constantino

Undergraduate Thesis Project
