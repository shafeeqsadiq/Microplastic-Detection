# Microplastic Detection using YOLOv5 🔍

A deep learning project to detect microplastics in images using YOLOv5 object detection model.

## Project Overview 📋

This project implements a microplastic detection system using YOLOv5, capable of identifying and localizing microplastic particles in images. The model was trained on a custom dataset and deployed as a web application using Flask.

## Technologies Used 🛠️

- **Deep Learning Framework**: YOLOv5
- **Programming Language**: Python 3.10
- **Training Platform**: Google Colab (GPU)
- **Web Framework**: Flask
- **Libraries**:
  - PyTorch
  - OpenCV
  - NumPy
  - Flask
  - Ultralytics YOLOv5

## Project Structure 📁

```
microplastic_detector/
├── app.py                 # Flask web application
├── best.pt               # Trained YOLOv5 model
├── requirements.txt      # Project dependencies
├── templates/            # HTML templates
│   └── index.html       # Web interface
└── data/                # Dataset configuration
    └── microplastics.yaml
```

## Model Training 🔨

### Dataset Preparation
- Custom dataset with annotated microplastic images
- Data split: Training (74%) and Validation (26%)
- Annotations converted from CSV to YOLO format

### Training Configuration
- **Model**: YOLOv5s (small variant)
- **Image size**: 640x640
- **Batch size**: 16
- **Epochs**: 50
- **Training Platform**: Google Colab with GPU acceleration

### Training Process
1. Dataset organization in YOLO format
2. Model configuration using microplastics.yaml
3. Training with YOLOv5 for 50 epochs
4. Model validation and performance metrics

## Model Performance 📊

- **mAP50**: 0.68796 (68.8%)
- **Precision**: 0.79481 (79.5%)
- **Recall**: 0.64218 (64.2%)

## Local Deployment 💻

### Prerequisites
```
# Python 3.10 required
python -m pip install -r requirements.txt
```

### Running the Web App
```
python app.py
```
Access the web interface at `http://localhost:5000`

## Usage Guide 📖

1. Start the Flask application
2. Access the web interface
3. Upload an image
4. Click "Detect" to process
5. View detection results

## Installation Steps 🔧

1. Download all the files from microplastic_detector

2. Install dependencies:
```
pip install -r requirements.txt
```

3. Activate the virtual environment:
   - On Windows:
     ```bash
     source yolov5_env/Scripts/activate
     ```

   - On macOS/Linux:
     ```bash
     source yolov5_env/bin/activate
     ```

4. Run the application:
```
python app.py
```

## Future Improvements 🚀

- Implement real-time detection
- Add support for video processing
- Improve model accuracy
- Deploy to cloud platform
- Add batch processing capability



## Project Assets

### Dataset and Model Files
⚠️ **Note**: Due to GitHub's file size constraints (>2GB), the full project files (dataset, trained models, and training outputs) are hosted on [Google Drive](https://drive.google.com/drive/folders/1m5EsVUZOsE2-a1QIdknnSO5P6vg35NwA?usp=sharing). 


[![Google Drive](https://img.shields.io/badge/Google%20Drive-4285F4?style=for-the-badge&logo=googledrive&logoColor=white)](https://drive.google.com/your-drive-link-here)



