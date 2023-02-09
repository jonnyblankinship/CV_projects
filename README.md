# CV_projects

This code uses the OpenCV library for Python to perform various image processing tasks. It includes several steps, including loading two images, resizing one of the images, adding a border to the resized image, making a region of interest (ROI) from the first image, converting the first image to grayscale, applying masks and bitwise operations to combine the two images, and counting the number of white, blue, and gold pixels in the final image.

Dependencies

- OpenCV (cv2)
- NumPy
- IPython's display
- Pillow (PIL)
- Google Colab patches (cv2_imshow)

Steps Involved

- Load two images: The code first loads two images, "Logo.png" and "Mustang.png", from the "/content/drive/MyDrive/CS362V/Data/" directory.
- Resize the second image: The second image is resized to half its original size using the cv2.resize() function.
- Add a border to the resized image: A white border is added to the resized image using the cv2.copyMakeBorder() function.
- Create the ROI: A region of interest is created from the first image using the shape attribute.
- Convert to grayscale: The first image is converted to grayscale using the cv2.cvtColor() function.
- Apply masks and bitwise operations: The grayscale image is thresholded to create a binary mask, which is then inverted. Bitwise operations are performed        on the original images and masks to combine the two images.
- Count the number of white pixels: The number of white pixels in the final image is counted using NumPy's sum() function.
- Count the number of blue pixels: The second image and the resized image with the border are converted to grayscale, and binary masks are created. Bitwise operations are performed on the original images and masks to isolate and count the number of blue pixels.
- Count the number of gold pixels: The final image and the resized image with the border are thresholded using the cv2.inRange() function to create masks for gold pixels. Bitwise operations are performed on the original images and masks to isolate and count the number of gold pixels.
- The final processed image is saved as "Homework1.png".

Note: The file paths and other parameters used in the code might need to be changed based on the environment where the code is being run.
