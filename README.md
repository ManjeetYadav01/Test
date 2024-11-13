Project: Parallel Image Processing with OpenCV

Description:

This Python script leverages OpenCV and multiprocessing to efficiently process a set of JPG images in parallel. For each image, it:

Reads the Image: Loads the image from the specified directory.
Creates a Binary Mask: Generates a binary mask where pixels with all three color channels (RGB) exceeding 200 are set to 255, and others to 0.
Writes the Mask: Saves the binary mask as a PNG image (lossless format).
Counts Pixels: Calculates the total number of pixels with a value of 255 in the mask.
Parallel Processing: Distributes the image processing tasks across multiple CPU cores using multiprocessing for faster execution.
Logs Total Pixel Count: Prints the cumulative count of pixels with a value of 255 across all processed images.

Requirements:
Python
OpenCV
NumPy
Multiprocessing
Installation:

Install Required Packages:
Bash
pip install opencv-python numpy multiprocessing
Use code with caution.

Usage:
Replace the Image Directory: 
Modify the image_dir variable in the main function to point to the directory containing your JPG images.

Execute the file:
test.ipynb

Output:
The script will create PNG files for each input image, representing the binary masks. The total count of pixels with a value of 255 across all masks will be printed to the console.

Additional Notes:
For large datasets, consider further optimization techniques like asynchronous programming or GPU acceleration.
Adjust the threshold value (200) to suit your specific image processing needs.
Experiment with different output formats and compression levels to balance image quality and file size.

License:
This code is released under the MIT License.
