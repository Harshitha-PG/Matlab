# Vegetation Detection from Satellite Images using MATLAB

## Overview

This project focuses on detecting vegetation from satellite images using MATLAB. The goal is to analyze satellite imagery to identify and classify vegetation regions based on various spectral bands and indices. The project employs image processing and classification techniques to accurately detect vegetation cover.

## Features

- Satellite image preprocessing (e.g., noise reduction, enhancement)
- Vegetation index calculation (e.g., NDVI, EVI)
- Vegetation classification using machine learning models
- Visualization of detected vegetation regions on satellite imagery
- Model evaluation metrics

## Prerequisites

Before running the code, make sure to have the following:

- MATLAB (version 2019b or higher recommended)
- Image Processing Toolbox
- Statistics and Machine Learning Toolbox
- Access to satellite images (e.g., Landsat or Sentinel data)

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/Vegetation-Detection-from-Satellite-Images-using-MATLAB.git
    ```

2. Navigate to the project directory:
    ```bash
    cd Vegetation-Detection-from-Satellite-Images-using-MATLAB
    ```

3. Ensure you have all the required toolboxes in your MATLAB environment.

## Usage

1. **Preprocessing the Images**: Use the `preprocessImage.m` script to load and preprocess satellite images, including noise reduction and enhancement.
   
2. **Calculate Vegetation Indices**: Use the `calculateNDVI.m` script to compute the Normalized Difference Vegetation Index (NDVI) or `calculateEVI.m` for Enhanced Vegetation Index (EVI).

3. **Classification**: Use the `classifyVegetation.m` script to classify the vegetation regions based on the selected index (NDVI/EVI). This can involve using thresholding or machine learning classification algorithms.

4. **Visualization**: Use `visualizeVegetation.m` to display the original image alongside the vegetation regions detected.

Example command for running the NDVI calculation:
```matlab
image = imread('satellite_image.jpg');
ndvi = calculateNDVI(image);
imshow(ndvi, []);
title('NDVI Image');
```
## File Structure

- `preprocessImage.m` - Image preprocessing script.
- `calculateNDVI.m` - Computes NDVI from the satellite image.
- `calculateEVI.m` - Computes EVI from the satellite image.
- `classifyVegetation.m` - Classifies vegetation regions.
- `visualizeVegetation.m` - Visualizes the vegetation classification.
- `data/` - Folder containing satellite images.

## Contributing

Feel free to contribute to the project by forking the repository, creating an issue, and submitting pull requests. Please ensure that your code follows the existing coding style and is well-documented.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Satellite image datasets from [NASA](https://www.nasa.gov/) and [ESA](https://www.esa.int/).
- MATLAB and Image Processing Toolbox for advanced image processing features.
