# k-Compress: Image Compression Using KMeans Clustering
## Overview
k-Compress is a Python-based image compression tool that uses the KMeans clustering algorithm. The project applies the **Elbow Method** to determine the optimal number of clusters and compresses an image by reducing the number of colors while preserving visual quality. This technique can significantly reduce the file size of images, making it a useful tool for image storage and transmission.

## Features
+ KMeans Clustering for image compression.
+ Elbow Method to find the optimal number of clusters.
+ Visualization of both the original and compressed images.

## Methodology
## **KMeans Clustering:**

+ The pixel values of the image are reshaped and converted to a float32 format for efficient clustering.
+ KMeans clustering is applied, where each pixel is replaced by the nearest color cluster center.

## Elbow Method:

+ The optimal number of clusters is determined using the Elbow Method, which helps minimize the within-cluster sum of squares (WCSS).
+ In this project, the optimal number of clusters (n=5) was found after testing.

## Image Compression:

+ The compressed image is generated by replacing each pixel with its corresponding cluster center.
+ The compressed image is then converted back to uint8 to minimize its size.

## Dependencies
To run the project, ensure you have the following Python libraries installed:

+ numpy
+ matplotlib
+ scikit-learn
+ CV2

## View Results:

+ The Elbow Method plot will show the optimal number of clusters.

![image](https://github.com/user-attachments/assets/3ea42f06-48cb-4637-b6da-335e2bdeb09b)


+ The compressed image will be displayed next to the original image for comparison.

![image](https://github.com/user-attachments/assets/2eeba122-523f-4baf-9c71-357fa9688ffd)


## Future Improvements
+ Implement advanced color quantization techniques for even better compression.
+ Add an interactive UI to select the number of clusters.
+ Extend the tool to compress videos.

## Contributing
Feel free to fork this project, submit issues, and create pull requests!

