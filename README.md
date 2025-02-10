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


microplastic_detector/
├── app.py                 # Flask web application
├── best.pt               # Trained YOLOv5 model
├── requirements.txt      # Project dependencies
├── templates/            # HTML templates
│   └── index.html       # Web interface
└── data/                # Dataset configuration
    └── microplastics.yaml


## Model Training 🔨

### Dataset Preparation
- Custom dataset with annotated microplastic images
- Data split: Training (80%) and Validation (20%)
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

- **mAP50**: [Your mAP50 score]
- **Precision**: [Your precision score]
- **Recall**: [Your recall score]

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

3. Run the application:
```
python app.py
```

## Future Improvements 🚀

- [ ] Implement real-time detection
- [ ] Add support for video processing
- [ ] Improve model accuracy
- [ ] Deploy to cloud platform
- [ ] Add batch processing capability

## Contributing 🤝

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License 📄

[Your chosen license]

## Acknowledgments 👏

- Ultralytics for YOLOv5
- Google Colab for training resources
- [Any other acknowledgments]

## Contact 📧

[Your Name] - [Your Email]

Project Link: [Your repository URL]
```

Remember to:
1. Fill in the performance metrics from your training results
2. Add your contact information
3. Choose and add appropriate license
4. Update repository URL
5. Add any specific acknowledgments
6. Customize sections based on your project's specific features

