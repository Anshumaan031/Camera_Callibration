# Camera_Callibration
The process of estimating the parameters of a camera is called camera calibration.</br>

This means we have all the information (parameters or coefficients) about the camera required to determine an accurate relationship between a 3D point in the real world and its corresponding 2D projection (pixel) in the image captured by that calibrated camera.</br>

Typically this means recovering two kinds of parameters</br>

Internal parameters of the camera/lens system. E.g. focal length, optical center, and radial distortion coefficients of the lens.</br>
External parameters : This refers to the orientation (rotation and translation) of the camera with respect to some world coordinate system.</br>

<h2>The Goal of Camera Calibration</h2>
The goal of the calibration process is to find the 3×3 matrix K, the 3×3 rotation matrix \mathbf{R}, and the 3×1 translation vector \mathbf{t} using a set of known 3D points (X_w, Y_w, Z_w) and their corresponding image coordinates (u, v). When we get the values of intrinsic and extrinsic parameters the camera is said to be calibrated.</br>

In summary, a camera calibration algorithm has the following inputs and outputs</br>

Inputs : A collection of images with points whose 2D image coordinates and 3D world coordinates are known.</br>
Outputs: The 3×3 camera intrinsic matrix, the rotation and translation of each image.</br>
