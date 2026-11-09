# Forest Fire Detection Using CNN

A binary image-classification project that uses a Convolutional Neural Network (CNN) built with TensorFlow/Keras to classify forest images as **Fire** or **Non-Fire**.

## Project Objective

To build an educational computer vision model that identifies visible fire patterns in forest images using CNN.

## Repository Structure

```text
Forest-Fire-Detection/
│
├── fire_dataset/
│   ├── no/              # Images without fire
│   └── yes/             # Images showing fire
│
├── test_images/         # Images for prediction
├── artifacts/           # Generated model files (not committed)
│
├── forest_fire_detection.ipynb
├── requirements.txt
├── .gitignore
└── README.md
```

## Dataset Setup

The dataset is not included in this repository.

Add your images to the following folders:

- `fire_dataset/no` – Images without fire.
- `fire_dataset/yes` – Images showing fire.

Supported dataset image formats: JPG, JPEG, PNG.

## Technologies Used

- Python
- TensorFlow and Keras
- Convolutional Neural Network (CNN)
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Model Workflow

1. Import required libraries.
2. Load and validate the dataset.
3. Visualize sample images and class distribution.
4. Split data into training and validation sets.
5. Resize images to 224 × 224 pixels.
6. Apply image augmentation.
7. Build and train the CNN model.
8. Use ModelCheckpoint and ReduceLROnPlateau callbacks.
9. Evaluate model performance.
10. Generate a classification report and confusion matrix.
11. Save the trained model.
12. Predict fire or non-fire from new images.

## Model Evaluation

The model is evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

Run the notebook to generate the actual evaluation results.

## How to Run the Project

1. Clone the repository:

```bash
git clone https://github.com/GAnurupa/Forest-Fire-Detection.git
```

2. Open the project folder:

```bash
cd Forest-Fire-Detection
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Add the dataset to the `fire_dataset` folder.

5. Open Jupyter Notebook:

```bash
jupyter notebook
```

6. Open `forest_fire_detection.ipynb`.

7. Run all cells from top to bottom.

## Prediction

The trained CNN model predicts whether a given forest image contains fire or no fire.

The prediction output includes:
- Fire or Non-Fire classification.
- Prediction confidence percentage.
- Display of the input image.

## Future Improvements

- Develop a web application using Streamlit.
- Test the model using an independent dataset.
- Explore transfer learning techniques.
- Improve model generalization.

## Limitations

This is an educational image-classification prototype. Its performance depends on the quality and diversity of the dataset. It is not a replacement for professional forest fire monitoring systems.

## Author

**Anurupa Gurijala**