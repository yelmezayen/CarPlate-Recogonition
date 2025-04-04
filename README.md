# Number Plate Detection & OCR System

A robust system for detecting vehicle number plates and performing Optical Character Recognition (OCR) using computer vision and deep learning techniques.

## 📌 Key Features
- **Number Plate Detection**: Utilizes a pre-trained InceptionV3 model with custom bounding box regression.
- **OCR Integration**: Extracts text from detected plates using Tesseract OCR.
- **Dataset Handling**: Includes tools for data labeling, annotation conversion (XML to CSV), and dataset splitting.
- **Real-World Applications**: Traffic management, automated toll collection, law enforcement, and parking management.

## 🚀 Motives
- Improve efficiency in traffic violation identification and toll collection.
- Enhance security through stolen vehicle detection.
- Streamline parking management in urban areas.

## 🛠️ Project Architecture
1. **Data Preparation**:
   - Label images using Label Studio.
   - Convert XML annotations to CSV.
   - Split dataset into training (80%) and testing (20%) sets.
2. **Model Training**:
   - Fine-tune InceptionV3 for bounding box prediction.
   - Train with Mean Squared Error (MSE) loss and Adam optimizer.
3. **OCR Pipeline**:
   - Extract detected plate regions.
   - Recognize text using Tesseract.

## 📂 Dataset
- **Total Images**: 228
- **Characteristics**: Multiple angles, lighting conditions, and visible number plates.
- **Annotation**: Bounding boxes labeled as "Number Plate" using Label Studio.

## 🔧 Installation
### Dependencies
- Python 3.7+
- Libraries:
  ```bash
  pip install tensorflow keras label-studio pytesseract opencv-python pandas scikit-learn
  ```

## Data Labeling:
```bash
Import images into Label Studio and annotate plates.
Export annotations as XML files.
```

  
