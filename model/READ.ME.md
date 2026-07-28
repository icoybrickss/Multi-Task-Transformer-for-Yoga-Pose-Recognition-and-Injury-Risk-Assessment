# Model

This folder contains the pretrained model and supporting artifacts used for the research project **"Multi-Task Transformer for Yoga Pose Recognition and Injury Risk Assessment."**

## Pretrained Model & Artifacts

The complete trained model and preprocessing artifacts are available on Google Drive.

**Download:**

https://drive.google.com/drive/folders/1t6x20Bcnu6rk7pmjCvPedHh-8JOY01nF?usp=sharing

**Contents:**

- `multitask_yoga_transformer.pth`
- Feature scaler
- Landmark scaler
- Biomechanical scaler
- Pose label encoder
- Risk label encoder
- Additional preprocessing artifacts required for inference

These files are packaged as a ZIP archive because they exceed GitHub's recommended file size limits.

---

## Model Architecture

The pretrained model is a **Multi-Task Transformer** designed to perform three tasks simultaneously:

- Yoga Pose Classification
- Injury Risk Classification (Safe / Unsafe)
- Joint-Level Risk Localization

The model combines three sources of information:

- MediaPipe landmark sequences
- Biomechanical feature sequences
- Aggregated biomechanical statistics

These inputs are fused within a Transformer-based architecture to produce predictions for all three tasks.

---

## Usage

The pretrained model is automatically loaded by the **YogaSafe Slim Inference Notebook**.

Once downloaded, extract the ZIP archive and place the saved artifacts in the expected directory before running inference.

---

## Notes

- The model was trained using the processed MediaPipe Pose landmark dataset described in the `dataset/` directory.
- Training, evaluation, Leave-One-Participant-Out (LOPO) validation, and model generation are fully documented in the training notebook located in the `notebooks/` directory.
- The pretrained artifacts are hosted on Google Drive because they exceed GitHub's recommended file size limits.
