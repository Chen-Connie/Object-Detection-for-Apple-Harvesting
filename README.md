# Object Detection for Apple Harvesting

This project uses image-based object detection to identify apples in field photos, aiming to support automation in harvesting tasks. Built with MATLAB and trained on labeled datasets, it demonstrates basic image preprocessing and object detection using bounding boxes.

> Uploaded as part of a computer vision / agricultural automation initiative.

---

## Features

- Object detection using MATLAB’s Computer Vision Toolbox
- Labeled dataset of apple images
- Bounding box annotations in `.mat` format
- Separated train/test image folders
- Visual overlay of detection results

---

## Project Structure

```
apple_object_detection/
├── Object_Detection.m                    # Main detection script
├── apple_resized/
│   ├── train/                            # Training images
│   ├── test/                             # Test images and labels
│   │   ├── test_label.mat                # Bounding box data
│   │   └── test_imageLabelingSession.mat
```

---

## How to Run (MATLAB Required)

### Prerequisites

- MATLAB (2021a or later recommended)
- Computer Vision Toolbox

### Steps

1. Open MATLAB
2. Set the working directory to the project root:
   ```
   cd path/to/apple_object_detection
   ```
3. Open and run the script:
   ```
   open Object_Detection.m
   run
   ```

---

## Dataset Info

The dataset is split into:
- `train/`: Images for training (not labeled in this repo)
- `test/`: Images with ground-truth annotations in `.mat` files

Bounding boxes are likely stored in variables such as `gTruth`, `bbox`, or `imageFilenames`.

---

## Author

Created by **Man-Ning Chen**  
If you use or adapt this project, please give credit or reach out for collaboration.
