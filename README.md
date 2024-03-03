# Thermal Video Component Tracking with Frequency Analysis 
## Task
Use OpenCV with the [video](https://drive.google.com/file/d/1PWS2MoFphHwTwblN82QZZbYqEmycN0Jj/view?usp=sharing) provided to find components(4 or 8 connected components) in the video that have a frequency of 0-1 Hz. 
## Attempt
My code for this task is in task_code.ipynb in the Task folder of this repository.     

The code tracks 4 connected components in a video frame-by-frame(every 512 frames), analyzes their intensity, and computes the dominant frequency of intensity variations using Fast Fourier Transform (FFT).

## Requirements
The following versions were used for this mini-project: 
- python 3.12.0
- matplotlib==3.8.3
- numpy==1.26.3
- opencv-python==4.9.0.80
- pandas==2.1.4
- cvzone==1.6.1

## Output
- The program will process the video frame-by-frame, analyzing connected components and computing their dominant frequencies.
- After every 512 frames, tracked components and their dominant frequencies, will be printed.
- The processed video with overlay will be saved as 'Thresh_overlay_frame.mp4' in the same directory.
- After the video is stopped, a DataFrame containing the frame ranges, component labels, and dominant frequencies below 1 Hz will be displayed.
  
## Acknowledgement
I would like to express my gratitude to Prof. Nipun Batra for this opportunity. I also wish to thank the project lead, Mr. Rishiraj Adhikary, for responding to all my queries and giving me helpful advice and suggestions. These tasks motivated me to learn more about image processing and analog signals.
## References
-  [https://pyimagesearch.com/2021/02/22/opencv-connected-component-labeling-and-analysis/](https://pyimagesearch.com/2021/02/22/opencv-connected-component-labeling-and-analysis/)
-  [https://www.geeksforgeeks.org/python-opencv-connected-component-labeling-and-analysis/](https://www.geeksforgeeks.org/python-opencv-connected-component-labeling-and-analysis/)
-  [https://mpolinowski.github.io/docs/Development/Python/2022-09-17-python-video-processing/2022-09-17/#getting-video-information](https://mpolinowski.github.io/docs/Development/Python/2022-09-17-python-video-processing/2022-09-17/#getting-video-information)
-  [https://answers.opencv.org/question/189428/connectedcomponents-like-function-for-grayscale-image/](https://answers.opencv.org/question/189428/connectedcomponents-like-function-for-grayscale-image/)
-  [https://stackoverflow.com/questions/25735153/plotting-a-fast-fourier-transform-in-python](https://stackoverflow.com/questions/25735153/plotting-a-fast-fourier-transform-in-python)
-  [https://www.w3schools.com/python/python_lists.asp](https://www.w3schools.com/python/python_lists.asp)
-  [https://www.youtube.com/watch?v=voRFbl-GKGY](https://www.youtube.com/watch?v=voRFbl-GKGY)
-  [https://stackoverflow.com/questions/64837060/getting-fft-result-peaks-at-0-hz](https://stackoverflow.com/questions/64837060/getting-fft-result-peaks-at-0-hz)
