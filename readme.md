# Calibration procedures:

- Print out the CHESSBOARD.png by original size.

- Run in terminal:

$mkdir build

$cd build/

$cmake ..

$make

$./camera_calibration ../in_VID5.xml

- Show the chessboard before the camera until it recognize it.

- Press “g” key to do the calibration.

- After calibration press “u” to change between the original picture and the undistorsed one.

- Save the build/out_camera_data.xml file for use, it is the calibration parameters file.

# Parameter Settings:
- You can change the resolution of camera from /camera_calibration.cpp by the parameter: m_width and m_height.

- You can also print out the ASYMMETRIC_CIRCLES_GRID.png file for calibration. You have to change the following settings:

1. /in_VID5.xml: <BoardSize_Width>4</BoardSize_Width><BoardSize_Height>11</BoardSize_Height>

2. /in_VID5.xml: <Calibrate_Pattern>"ASYMMETRIC_CIRCLES_GRID"</Calibrate_Pattern>

- To switch to a different the camera: 

/in_VID5.xml <Input>"0"</Input>: change the camera ID number.
