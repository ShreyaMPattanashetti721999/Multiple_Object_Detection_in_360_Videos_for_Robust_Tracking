# Multiple Object Detection in 360° Videos for Robust Tracking

This project presents an efficient way to detect objects in 360° videos to enhance tracking performance. The focus is on detecting 'Person' and 'Car' classes using a specialized CNN network called YOLO360, which builds upon YOLOv3 through transfer learning. This project addresses challenges such as the unavailability of annotated datasets, geometric distortions at panoramic poles, and the high computational demands of processing high-resolution 360° media.

## Paper

The detailed methodology, experiments, and results are documented in the paper titled "Multiple Object Detection in 360° Videos for Robust Tracking." You can find the paper in this repository as `My360YOLOPaper.pdf`.

## Project Structure

- `Published360YOLOPaper.pdf`: The research paper detailing the entire project.
- `data/`: Directory containing the annotated dataset used for training.
- `models/`: Pre-trained models and weights for YOLO360.
- `notebooks/`: Jupyter notebooks for training, evaluation, and experimentation.
- `scripts/`: Python scripts for preprocessing, training, and evaluation.

## Key Components

### Dataset

The dataset comprises annotated 360° video frames with ground truth object positions. The frames are extracted from various 360° videos, and objects are manually annotated for 'Person' and 'Car' classes.

### YOLO360

YOLO360 is a modified version of YOLOv3, optimized for 360° videos. The model is trained using transfer learning with manually annotated datasets to handle geometric distortions and other challenges unique to 360° videos.

### Object Tracking

Object tracking is performed using SORT and DEEP SORT algorithms. These algorithms are enhanced by the improved object detection capabilities of YOLO360, resulting in better tracking accuracy and precision.

## Usage
Clone this repository to your local machine.
Install the required packages using the requirements.txt file.
Download the YOLOv3 weights and place them in the models/ directory.
Download the spaCy English model.
Open the Jupyter notebooks in the notebooks/ directory in your preferred environment (e.g., Jupyter Lab, Jupyter Notebook).
Follow the instructions and run the cells sequentially to reproduce the results.

## Results
The results of the object detection and tracking experiments are presented in the paper and the Jupyter notebooks. Key metrics include MOTA (Multiple Object Tracking Accuracy) and MOTP (Multiple Object Tracking Precision), demonstrating the improved performance of YOLO360 over traditional YOLOv3 in 360° video contexts.

## Installation

To run the project, you need to have Python installed along with several packages. You can install the required packages using the following command:

```bash
pip install -r requirements.txt
