# -Motion-Detector-OpenCV

Problem Statement : 
You have been approached by a company that is studying human bahavior. Your task is to give them a webcam, that can detect the motion or any movement in front of it. This should return a graph, this graph should contain for how long the human/object was in front of the camera.

Solution Logic : 


Additional Python Libraries Required :
OpenCV
   pip install opencv-python
Pandas
   pip install pandas
Bokeh
  pip install bokeh
Analysis of all Windows :
After running the code there 4 new window will appear on screen.

1. Gray Frame:
In Gray frame the image is a bit blur and in grayscale we did so because, In gray pictures there is only one intensity value whereas in RGB(Red, Green and Blue) image thre are three intensity values. So it would be easy to calculate the intensity difference in grayscale.
2. Difference Frame:
Difference frame shows the difference of intensities of first frame to the current frame.
3. Threshold Frame:
If the intensity difference for a particular pixel is more than 30(in my code) then that pixel will be white and if the difference is less than 30 that pixel will be black.
4. Color Frame:
In this frame you can see the color images in color frame along with green contour around the moving objects.
Time Record of Movements :
The Time_of_movements file will be stored in the folder where your code file is stored. This file will be in csv extension. In this file the start time of motion and the end time of motion will be recorded.

Plotting Time Intervals :
Time Intervals will be plotted using Bokeh Plot. Bokeh is an interactive visualization library that targets modern web browsers for presentation. Here, the time intervals are collected by the csv file and then plotted using Bokeh. The green color shows that an object was under motion, time is displayed in milisecond(ms).

Usage :
The Repository contains 2 python files :

motion_detector.py :
It conatins the code for Motion Detection. By running this file you can detect the motion in front of webcam and can record the start and end time of motion.
plotting.py :
It makes use of Boken Library. By running this file you can plot the time intervals. This file imports the code of motion detection from motion_detector.py, so motion_detector.py needs to be in same directory.
References:
https://www.youtube.com/watch?v=-ZrDjwXZGxI
