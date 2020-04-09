# openCV-smoothing-
Homework for DIP class in Tongji University by ( 1656039 ) for April 6th 2020
Used openCV python3.8 ,numpy and matplotlib
Showed 2D convolution ,BLur ,Gaussian-Blur ,Median Blur(For noisy images) and Bilatrealfill(For pepper and salt images)
Check OpenCV documentation--https://docs.opencv.org/master/d4/d13/tutorial_py_filtering.html
For kernel used Wikipedia--https://en.wikipedia.org/wiki/Kernel_(image_processing)


kernel = np.ones((5, 5), np.float32)/25
dst = cv2.filter2D(img, -1, kernel)
blur = cv2.blur(img, (5, 5))
gblur = cv2.GaussianBlur(img, (5, 5), 0)
median = cv2.medianBlur(img, 5)
bilateralFilter = cv2.bilateralFilter(img, 9, 75, 75)
