# Solution to option 1
The algorithm that I managed to get to was to essentially segment the paper out from the carpet. This is done by getting the largest contour which ends up being the paper. We than extract the QR code and create an ROI that encloses those contours. From there we generate points for each of the three squares that compose a QR code and can figure if the points are in the correct position. If not we can figure out based on the four total cases the points can be in and find the angle needed to correct the skew of the resulting bounding box.

For calculating distance we use the cameras properties to figure out the ratio of the size of the paper to pixels which allows us to get an estiamate on the distance from the camera to the pattern.

My goal from that was to figure out the angle of the camera and the picture and than be able to figure out the x and y components and from there be able to get the camera's orientation.

