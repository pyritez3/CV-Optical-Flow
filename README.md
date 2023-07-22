# Optical Flow

Optical flow is a computer vision technique that allows us to understand how objects in a scene are moving and changing over time. This information can be used for various tasks, such as object tracking, video stabilization, and generating visual effects.

## Lucas-Kanade Method

The first part of the code demonstrates the use of the Lucas-Kanade method to estimate optical flow for a sequence of frames. The Lucas-Kanade algorithm is a local optical flow approach, assuming constant motion within small regions. It tracks points in the frame using the ShiTomasi corner detection and calculates the optical flow between consecutive frames. The flow vectors are then visualized as tracks on the video. The Lucas-Kanade method is well-suited for small displacements and minor changes in illumination.

## Gunnar-Farneback Optical Flow

The second part of the code showcases the Gunnar-Farneback optical flow algorithm, a dense optical flow approach. Unlike the Lucas-Kanade method, this algorithm estimates motion for all pixels in the frame. It provides a more comprehensive view of the motion within the video. The Gunnar-Farneback method can handle larger displacements and changes in illumination but is computationally more intensive.

## Usage

1. Make sure you have the necessary libraries installed (OpenCV).
2. Replace the file path "/content/car1.mp4" with the path to your video file.
3. Run the code to visualize the optical flow using both methods. You can press 'ESC' to exit the video playback.

Note: This code is designed for use in Google Colab, but you can adapt it for other environments.

Feel free to use and modify this code for your own optical flow tasks or research. Happy coding!
