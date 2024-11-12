


# Image Feature Extraction and Time Series Prediction

This project focuses on extracting features from images in a video sequence, preprocessing the data, and using it to build a time-series prediction model. The goal is to create a model that can predict future data points by analyzing extracted image features.

## Steps and Workflow

### 1. Image Preprocessing
- **Video to Image Sequence Conversion**: Convert a video into a sequence of images with filenames in sequential order (e.g., `1.jpg`, `2.jpg`, ...).
- **Grayscale Conversion**: Apply grayscale conversion to all images.
- **Image Feature Extraction**: 
  - Use image processing techniques like denoising, blurring, and sharpening.
  - Extract features related to snow (if applicable), using both direct extraction and masking techniques.

### 2. Algorithm Development and Validation
- **Algorithm Conceptualization**: Design an algorithm to identify and validate extracted features.
- **Validation**: Ensure the algorithm achieves at least 80% accuracy.

### 3. Numeric Feature Extraction
- Extract numeric features from the processed images to create a dataset.
- Build a function for numeric feature extraction to streamline this process.

### 4. Dataset Creation
- Use the function created in Step 3 to build a structured numeric dataset for analysis and modeling.

### 5. Data Preparation
- **Data Import**: Import the dataset created in Step 4.
- **Data Cleaning**: Remove any outliers, fillers, and missing values.
- **Data Analysis**:
  - Analyze the distribution of the data.
  - Check the correlation matrix to assess relationships between variables.
  - Conduct ANOVA testing to identify significant features (p-values).

### 6. Data Normalization
- Normalize the dataset for improved model performance.

### 7. Model Training and Evaluation
- **Model Selection**: Experiment with time series models such as ARIMA and LSTM+RNN.
- **Data Splitting**: Split the data into training (80%) and testing (20%) sets.
- **Model Evaluation**: Evaluate the model's accuracy on both training and testing data.
- **Model Selection**: Choose the best-performing model for further use.

### 8. Prediction and Future Data Generation
- **Future Prediction**: Use the chosen model to generate predictions for the next 50 data points.
- **Model Persistence**: Save the final model using pickling for future use.

## Dependencies

This project requires the following libraries:
- Python (version 3.x)
- OpenCV (for image processing)
- NumPy and Pandas (for data handling)
- Scikit-learn (for model evaluation and preprocessing)
- Statsmodels (for ARIMA modeling)
- TensorFlow/Keras (for LSTM and RNN models)

## Usage

1. Clone the repository.
2. Follow the image preprocessing steps outlined in the notebook or scripts.
3. Use the provided functions to extract and preprocess features.
4. Train and evaluate the model on the dataset.
5. Run the prediction script to generate future data points.

## Results

- The Image Segmentation model should be capable of achieving 80%+ accuracy on the validation set.
- Future data predictions can be generated approximately 50 rows ahead, or else they go for only 10 rows ahead, with validation accuracy for min 85% to 90%.


