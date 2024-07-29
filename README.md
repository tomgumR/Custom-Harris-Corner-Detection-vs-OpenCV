# Custom-Harris-Corner-Detection-vs-OpenCV
Implementation of Harris Corner Detection from Scratch and Comparison with OpenCV to Detect Corners


Implementation of Harris Corner Detection from Scratch and Comparison with OpenCV to Detect Corners

Author
Tammy L. Ralte 

Project Overview
This project demonstrates the implementation of the Harris Corner Detection algorithm from scratch and compares it with OpenCV's built-in implementation. The goal is to detect key feature points in images, which is crucial for various image processing tasks such as image stitching.

AIM: The aim of this project was to apply our theoretical understanding of Harris Corner Detection, as taught in our class, by implementing it from scratch and evaluating its performance in comparison to OpenCV's built-in Harris Corner Detection function.


Dependencies
* Python 3.x
* OpenCV
* NumPy
* Matplotlib
* Scipy
  
Setup
1. Install required packages:   pip install opencv-python-headless numpy matplotlib scipy 
2. Mount Google Drive (if using Google Colab): from google.colab import drive
3. drive.mount('/content/drive')
4. Navigate to the project directory: cd /content/drive/MyDrive/CV/Question 1
   

Steps for Harris Corner Detection
1. Import the Required Libraries: Import necessary libraries such as OpenCV, NumPy, Matplotlib, and Scipy.
2. Load Images: Load the images from the specified directory.
3. Define the Gaussian Kernel: Create a 2D Gaussian kernel for gradient smoothing.
4. Implement the Sobel Operator: Calculate gradients in both the x and y axes using the Sobel operator.
5. Calculate Harris Corner Response: Using the Harris corner detection algorithm, calculate the Harris corner response for every pixel to detect corners.
6. Set a Threshold: Apply a threshold to the corner response function to identify significant corners.
7. Identify and Mark Corners: Mark the detected corners with green circles on the original image.
8. Display Results: Display the original image, the image with corners detected using the custom implementation, and the image with corners detected using OpenCV's built-in function.


**Method Descriptions**
Gaussian Kernel
Generates a Gaussian kernel used for smoothing the image to reduce noise.

Method: def gaussian_kernel(size=3, sigma=1)

Sobel Operator
Applies the Sobel operator to compute image gradients in both x and y directions.

Method: def apply_sobel_operator(image)

Custom Harris Corner Detection
Implements the Harris Corner Detection algorithm from scratch to detect corners in an image.

Method: def detect_harris_corners(image_path, k=0.04, threshold_ratio=0.01)

Processing Images from Folder
Processes all images in a specified folder to detect corners using both the custom and OpenCV implementations.

Method: def process_images_from_folder(folder_path)


Running the Code
1. Specify the folder path: pythonCopy code  folder_path = '/content/drive/MyDrive/CV/Question 1'
   
2. Process the images in the folder: pythonCopy code  process_images_from_folder(folder_path)
   
  
Conclusion
This project demonstrates the implementation of the Harris Corner Detection algorithm from scratch and its comparison with OpenCV's built-in implementation. The visualization helps to understand the differences and effectiveness of both methods in detecting corners in images.


