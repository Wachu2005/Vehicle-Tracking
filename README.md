# Vehicle Detection and Tracking with Storing coordinates in CSV file.


## Discription

The objective of my project was to detect different vehicles (car, bike, bus) and store their X and Y coordinates to make futher script that check if the student gone over the line.
I annotated single frames from video sample to get data for training.
I used a YOLOv7 model for this task. I trained the model with over 100 images using batch size of 8 and about 500 epochs in total.
After All from  the prediction matrixes for every frame i extracted the X and Y coordinates, class name and saved them in CSV using pandas. 




## DEMO

![Alt Text](https://github.com/Wachu2005/Vehicle-Tracking/blob/master/ezgif.com-video-to-gif%20(1).gif)

![Alt Text](https://github.com/Wachu2005/Vehicle-Tracking/blob/master/ezgif.com-video-to-gif.gif)
## Tech Stack

**Python**

**OpenCV**

**Jupyter Notebook**

**Google Colab**

**RoboFlow**

**PyTorch**

**Pandas**

**Numpy**
