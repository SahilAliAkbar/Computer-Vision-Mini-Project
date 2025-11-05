# Computer Vision Project

## Course Information
**Course:** Computer Vision (21CSE454T)  
**Presented To:** Mr. Vinoth K - 103672

## Team Members
- **Kundan Ratakonda** - RA2211026010055
- **Sahil Ali Akbar** - RA2211026010055

---

## Project Overview

This repository contains implementations of various computer vision techniques divided into two main units:

### Unit 1: Image Filtering and Noise Reduction (MATLAB)
Implementation of multiple filtering techniques to reduce Gaussian noise in images.

### Unit 2-5: Advanced Image Analysis (Python/OpenCV)
Comprehensive implementation of shape detection, region analysis, motion tracking, and pedestrian detection.

---

## Unit 1: Image Filtering Techniques

### Description
This unit demonstrates various filtering methods to remove Gaussian noise from images using MATLAB.

### Features
- **Noise Addition:** Adds Gaussian noise to the original image
- **Filter Implementations:**
  - Wiener Filter
  - Median Filter
  - Gaussian Filter
  - Mean Filter
  - Bilateral Filter
  - Low-pass Filter
  - High-pass Filter
  - Laplacian Filter

### Visualization
Each filter output is displayed with:
- Filtered image
- Corresponding histogram

### Requirements
- MATLAB with Image Processing Toolbox
- Test image: `cameraman.tif`

### Usage
```matlab
% Run the script
Unit_1.m
```

### Output
The script generates 10 figures:
1. Original image and histogram
2. Noisy image and histogram
3-10. Each filter result with histogram

---

## Unit 2-5: Advanced Computer Vision Techniques

### Unit 2: Shape and Region Analysis

#### Features
- Connected component analysis
- Object labeling and counting
- Area and perimeter calculation
- Centroid detection
- Bounding box visualization

#### Implementation Details
- Automatic thresholding using Otsu's method
- 8-connectivity component analysis
- Comprehensive object statistics table

---

### Unit 3: Hough Transform Detection

#### Features
- **Line Detection:**
  - Uses Hough Line Transform (Probabilistic)
  - Adjustable parameters for line sensitivity
  
- **Circle Detection:**
  - Hough Circle Transform implementation
  - Tuned parameters for accurate circle detection
  - Configurable radius ranges

#### Parameters
- `minLineLength`: 100
- `maxLineGap`: 10
- `minRadius`: 30
- `maxRadius`: 70

---

### Unit 4: Optical Flow and Motion Analysis

#### Features
- Farneback optical flow implementation
- Motion vector visualization
- HSV color mapping for direction and magnitude
- Frame-by-frame motion tracking

#### Implementation Details
- `pyr_scale`: 0.5
- `levels`: 3
- `winsize`: 15
- Sample frames captured every 20 frames

#### Input Requirements
- Video file (MP4/AVI format)
- Recommended size: Under 10-20 MB

---

### Unit 5: Pedestrian Detection

#### Features
- HOG (Histogram of Oriented Gradients) descriptor
- Pre-trained SVM classifier
- Multi-scale detection
- Bounding box visualization

#### Implementation Details
- Uses OpenCV's default people detector
- `winStride`: (4, 4)
- `padding`: (8, 8)
- `scale`: 1.05

---

## Installation and Setup

### Prerequisites
```bash
# For Python implementation
pip install opencv-python
pip install numpy
pip install matplotlib
pip install pandas
```

### For Google Colab
All dependencies are pre-installed. Simply upload the notebook and run.

---

## Usage Instructions

### Unit 1 (MATLAB)
1. Ensure MATLAB is installed with Image Processing Toolbox
2. Place `cameraman.tif` in the working directory
3. Run the script: `Unit_1.m`

### Unit 2-5 (Python)
1. Open the notebook in Google Colab
2. Run cells sequentially
3. Upload images/videos when prompted
4. View results and analysis tables

---

## Expected Outputs

### Unit 1
- 10 figure windows showing original, noisy, and filtered images
- Histograms for each processing stage

### Unit 2
- Labeled objects with bounding boxes
- Object analysis summary table
- Centroid markers

### Unit 3
- Detected circles highlighted in blue
- Detected lines highlighted in green
- Combined visualization

### Unit 4
- Motion flow visualization in HSV color space
- Direction indicated by hue
- Magnitude indicated by brightness

### Unit 5
- Detected pedestrians with green bounding boxes
- Count of detected persons

---

## Technical Notes

### Image Preprocessing
- All color images converted to grayscale
- Gaussian blur applied for noise reduction
- Binary thresholding using Otsu's method

### Performance Considerations
- Video processing: Use shorter clips for faster results
- Circle detection: Adjust parameters based on object size
- Pedestrian detection: Works best with clear street scenes

---

## Troubleshooting

### Common Issues

**Unit 1:**
- Ensure image file path is correct
- Check if Image Processing Toolbox is installed

**Unit 2-5:**
- If shapes not detected, adjust threshold values
- For poor circle detection, modify `param2` value
- Video processing may be slow for large files
- Pedestrian detection requires clear, upright persons

---

## References

1. OpenCV Documentation: https://docs.opencv.org/
2. MATLAB Image Processing Toolbox
3. Histogram of Oriented Gradients for Human Detection (Dalal & Triggs, 2005)
4. Farneback Optical Flow Algorithm

---

## License

This project is submitted as part of academic coursework for Computer Vision (21CSE454T).

---

## Acknowledgments

Special thanks to **Mr. Vinoth K** for guidance and instruction throughout the course.

---

## Contact

For questions or issues, please contact:
- Kundan Ratakonda: RA2211026010055
- Sahil Ali Akbar: RA2211026010055
