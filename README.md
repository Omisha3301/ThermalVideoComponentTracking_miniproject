# ThermalVideo_miniproject_task
## TASK
Use OpenCV with the [video](https://drive.google.com/file/d/1PWS2MoFphHwTwblN82QZZbYqEmycN0Jj/view?usp=sharing) provided to find components(4 or 8 connected components) in the video that have a frequency of 0-1 Hz. 
## Attempt
My code for this task is in task_code.ipynb in the Task folder of this repository\
The code calculates the 8 connected components in a frame and then tracks the intensity of these areas for the next 511 frames, prints what it has tracked, and plots a frequency domain graph for each component tracked, then repeats the process.
#### Usage of mean intensity, instead of centroid's intensity
The centroid of the component detected in the first frame, might not have a significant intensity change in the consequent frames. However, the intensity of the areas covered by the rest of the component might change drastically which would not be detected.
#### Frequency domain graph
The list of intensity changes when read as a signal will be a nonperiodic signal and will not have a fixed frequency, a frequency domain graph could help identify which band of frequencies the signal has.
If most of the component's frequencies are in the 0-1Hz band then those can be selected (not implemented).
## Software Requirements
I have used the following versions for this mini-project: python 3.12.0, matplotlib==3.8.3, numpy==1.26.3, opencv-python==4.9.0.80
## Acknowledgement
I would like to express my gratitude to Prof. Nipun Batra for this opportunity. I also wish to thank the project lead, Mr. Rishiraj Adhikary, for responding to all my queries and giving me helpful advice and suggestions. These tasks motivated me to learn more about image processing.
## References
-  [https://pyimagesearch.com/2021/02/22/opencv-connected-component-labeling-and-analysis/](https://pyimagesearch.com/2021/02/22/opencv-connected-component-labeling-and-analysis/)
-  [https://www.geeksforgeeks.org/python-opencv-connected-component-labeling-and-analysis/](https://www.geeksforgeeks.org/python-opencv-connected-component-labeling-and-analysis/)
-  [https://mpolinowski.github.io/docs/Development/Python/2022-09-17-python-video-processing/2022-09-17/#getting-video-information](https://mpolinowski.github.io/docs/Development/Python/2022-09-17-python-video-processing/2022-09-17/#getting-video-information)
-  [https://answers.opencv.org/question/189428/connectedcomponents-like-function-for-grayscale-image/](https://answers.opencv.org/question/189428/connectedcomponents-like-function-for-grayscale-image/)
-  [https://stackoverflow.com/questions/25735153/plotting-a-fast-fourier-transform-in-python](https://stackoverflow.com/questions/25735153/plotting-a-fast-fourier-transform-in-python)
-  [https://www.w3schools.com/python/python_lists.asp](https://www.w3schools.com/python/python_lists.asp)
