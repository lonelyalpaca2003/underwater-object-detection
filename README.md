# underwater-object-detection

# Underwater Object Detection

Object detection for underwater creatures using YOLOv26n.

## What it does

Detects 7 types of marine life in images:
- Fish
- Jellyfish
- Penguin
- Puffin
- Shark
- Starfish
- Stingray

## Dataset

Uses the [Aquarium Data COTS dataset](https://www.kaggle.com/datasets/slavkoprytula/aquarium-data-cots) from Kaggle.

## Results

| Class | Precision | Recall | mAP@0.5 | mAP@0.5:0.95 |
|-------|-----------|--------|---------|--------------|
| All | 0.768 | 0.652 | 0.718 | 0.435 |
| Fish | 0.793 | 0.686 | 0.755 | 0.425 |
| Jellyfish | 0.882 | 0.868 | 0.926 | 0.522 |
| Penguin | 0.657 | 0.596 | 0.611 | 0.272 |
| Puffin | 0.661 | 0.432 | 0.557 | 0.294 |
| Shark | 0.826 | 0.582 | 0.705 | 0.452 |
| Starfish | 0.810 | 0.704 | 0.731 | 0.522 |
| Stingray | 0.748 | 0.697 | 0.742 | 0.556 |

## Setup

Install dependencies with uv:
```bash
uv sync
```

Download the dataset from Kaggle and update the paths in the notebook.

## Running
```bash
uv run jupyter notebook notebook.ipynb
```

The notebook has the training code and evaluation.
