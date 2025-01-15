# Image Processing and Feature Extraction Project

This project focuses on image processing and feature extraction using various algorithms and techniques. The project is organized into multiple Jupyter notebooks, each serving a specific purpose in the overall workflow.

## Project Structure

```
1_Image_Process_V2.ipynb
1_Image_Process.ipynb
2_Image_Algo_Test.ipynb
3_POC_Feature_Extraction.ipynb
4_Gen_Dataset.ipynb
arbitrary/
data/
data_1/
data_2/
    dataset.csv
POC Map/
```

## Notebooks Overview

### 1. Image Processing

- **1_Image_Process.ipynb**: Initial image processing techniques and experiments.
- **1_Image_Process_V2.ipynb**: Updated version with refined image processing methods.
- These Extracts image frames of A Glacier which was sourced from Youtube for Testing , the video can be found [here](https://www.youtube.com/shorts/xiFXn2EcvXk).

### 2. Image Algorithm Testing

- **2_Image_Algo_Test.ipynb**: Testing various image processing algorithms. This notebook includes:
  - Loading and displaying images.
  - Applying thresholding and other preprocessing techniques.
  - Saving processed images.

### 3. Proof of Concept: Feature Extraction

- **3_POC_Feature_Extraction.ipynb**: Extracting features from images. This notebook includes:
  - Functions to calculate various features such as pixel intensity distribution, convex hull, and image dimensions.
  - Visualization of features using histograms and plots.

### 4. Generate Dataset

- **4_Gen_Dataset.ipynb**: Generating a dataset by extracting features from a set of images. This notebook includes:
  - Functions to extract features from images.
  - Saving the extracted features into a CSV file.

## Key Functions

### Feature Extraction Functions

- `Feature_1(image_path)`: Calculates pixel intensity distribution.
- `Feature_2(image_path)`: Applies convex hull processing and extracts features.
- `Feature_3(image_path)`: Combines cropping and feature extraction.
- `Feature_4()`: Calculates the diagonal length of the image.
- `Feature_5()`: Returns the width of the image.
- `Feature_6()`: Returns the height of the image.
- `Feature_7()`: Calculates threshold and histogram of pixel intensities.

### Utility Functions

- `draw_line(r1, c1, r2, c2)`: Generates pixel coordinates for a straight line between two points.
- `crop(image_path)`: Applies convex hull processing and crops the region inside the convex hull.

## Dataset Generation

The dataset generation process involves extracting features from images and saving them into a CSV file. The features are extracted using the `Feature` function, which combines multiple feature extraction methods.

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

## Results

- The Image Segmentation model should be capable of achieving 80%+ accuracy on the validation set.
- Future data predictions can be generated approximately 50 rows ahead, or else they go for only 10 rows ahead, with validation accuracy for min 85% to 90%.

## How to Run

1. Clone the repository.
2. Install the required dependencies.
3. Open the Jupyter notebooks in your preferred environment.
4. Run the cells to execute the code and generate the dataset.

## Dependencies

- Python 3.x
- OpenCV
- NumPy
- Matplotlib
- Seaborn
- Scikit-image
- PIL (Pillow)
- SciPy

## Example Usage

```python
# Example usage of Feature_1 function
image_path = "path/to/image.jpg"
feature_value = Feature_1(image_path)
print(feature_value)
```

## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue if you have any suggestions or improvements.

## License

This project is licensed under the MIT License.

## Contact

For any queries, reach out to:

- Name: Harsh Mahanti  
  Email: mahantiharsh@gmail.com

- Name: Roumo Kundu  
  Email: rjroumo@gmail.com






