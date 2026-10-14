# ☀️ Solar Filament Instance Segmentation Using YOLO

## 📌 Project Overview

This project focuses on detecting and segmenting solar filaments in solar imagery using a YOLO-based instance segmentation pipeline. Solar filaments are elongated structures visible on the Sun's surface, and accurately identifying them can be challenging because of their thin shapes, varying sizes, and complex backgrounds.

The project uses a tiled image-processing approach to help the model analyze high-resolution solar images in smaller regions, potentially improving its ability to identify fine structures.

This work was developed as part of a Kaggle-based machine learning workflow.

## 🎯 Objectives

- Detect solar filaments in solar images.
- Perform instance segmentation to identify individual filament regions.
- Apply tiled image processing to handle high-resolution imagery.
- Generate segmentation predictions for evaluation and visualization.
- Explore deep learning techniques for solar image analysis.

## 🛠️ Technologies Used

- **Python** — Core programming language
- **Jupyter Notebook** — Development and experimentation
- **YOLO** — Object detection and instance segmentation
- **NumPy** — Numerical computations
- **Pandas** — Data handling and preprocessing
- **OpenCV / PIL** — Image processing, where applicable
- **Matplotlib** — Visualization
- **Kaggle** — Dataset access and experimentation environment

## 🔬 Methodology

The pipeline is organized around the following stages:

### 1. Data Preparation
Load the solar imagery and associated annotations or masks, and prepare the data for model processing.

### 2. Image Tiling
Divide large solar images into smaller tiles so that fine structures can be processed at a more manageable resolution.

### 3. YOLO-Based Segmentation
Use a YOLO instance segmentation model to identify solar filament regions and generate segmentation predictions.

### 4. Prediction Processing
Process predictions from individual tiles and, where implemented, map the predicted regions back to their original image coordinates.

### 5. Visualization and Evaluation
Visualize the resulting segmentation masks and evaluate model performance using the metrics supported by the notebook.

## 📂 Repository Structure

```text
Solar_Filament_Instance_Segmentation/
│
├── yolo_tiled_solar_pipeline.ipynb
└── README.md
```

Additional scripts, configuration files, model weights, or dataset instructions can be added as the project develops.

## 🚀 Getting Started

### Prerequisites

- Python 3.x
- Jupyter Notebook or JupyterLab
- The Python libraries required by the notebook
- Access to the relevant Kaggle dataset
- Model weights and configuration files, if required by the pipeline

### Installation

Clone the repository:

```bash
git clone https://github.com/AbdielMagdi/Solar_Filament_Instance_Segmentation.git
```

Navigate to the project directory:

```bash
cd Solar_Filament_Instance_Segmentation
```

Install the dependencies required by the notebook. For example:

```bash
pip install numpy pandas matplotlib opencv-python pillow jupyter
```

Install the appropriate YOLO package and version based on the imports and model implementation in the notebook.

### Running the Notebook

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open `yolo_tiled_solar_pipeline.ipynb` and execute the cells in sequence.

**Note:** Configure the dataset paths, model weights, and other input paths according to your local environment or Kaggle notebook environment before running the pipeline.

## 📊 Expected Output

Depending on the notebook configuration, the pipeline may produce:

- Solar filament segmentation predictions.
- Predicted instance masks or segmentation overlays.
- Visualizations of detected solar structures.
- Evaluation results and other model outputs.

Actual outputs depend on the dataset, model configuration, and evaluation procedure used.

## 🌞 Applications

Solar filament segmentation can support research in solar physics by helping researchers identify and analyze filament structures in solar observations. Automated segmentation can also assist with large-scale solar image analysis.

## 🔮 Future Improvements

- Experiment with different YOLO model configurations.
- Optimize tile size and overlap strategies.
- Improve segmentation of thin and faint filaments.
- Evaluate predictions using suitable segmentation metrics.
- Explore inference optimization for high-resolution solar imagery.

## 👨‍💻 Author

**Abdiel Magdi**

GitHub: [@AbdielMagdi](https://github.com/AbdielMagdi)

## 📄 License

MIT License

Copyright (c) 2026 Abdiel Magdi

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
