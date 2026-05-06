# Real-Time-Child-Identification-and-Tracking-System
A Multi-Stage Deep Learning and Computer Vision Framework for Robust Child Identification in Kindergarten (ICIET 2026 **Under Publication**)

---

A real-world pipeline for identifying and tracking children in kindergarten CCTV footage using face recognition and temporal consistency.

**Identification Accuracy: 78.78%**  
**Detection Rate: 97.54%**  
**~2× improvement over baseline (39.33%)**

---

## Why This Problem is Challenging

Child identification in CCTV footage is challenging due to:

- Occlusions and partial visibility  
- Non-frontal poses  
- Motion blur and low resolution  
- Continuous movement and interaction  

Traditional systems rely on single-frame predictions, leading to unstable identity assignment.

---

## How This System Solves It

This system improves stability by combining:

- Detection + Tracking  
- Face Recognition  
- Temporal Consistency  

Instead of making decisions per frame, identity is stabilized across multiple frames.

---

## System Overview

![System Pipeline](images/system_pipeline.png)

Main stages:

1. Body Detection (YOLOv8)  
2. Tracking (SORT)  
3. Face Detection (DSFD)  
4. Embedding Extraction (FaceNet512)  
5. Temporal Buffering  
6. Identity Matching  
7. Voting & Stabilization  

---

## Detailed Documentation

- [Dataset Description](docs/dataset_description.md)
- [System Pipeline](docs/system_pipeline.md)
- [Tracking & Temporal Logic](docs/tracking_and_temporal_logic.md)
- [Results & Evaluation](docs/results_and_evaluation.md)
- [Limitations & Future Work](docs/limitations_and_future_work.md)
