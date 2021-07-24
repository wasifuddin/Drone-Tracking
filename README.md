# Drone-Tracking
CVZone Competition

###Steps done to get the output result:

- First I have created a custom dataset by extracting some frames from the given video
- Then I trained the dataset for 300 epochs using yolov5
- After that I did tracking on the video using the trained weights and yolov5 deepsort algortihm
- To prevent duplicate counting and smoothen out the tracking I modified two files track.py and deep_sort.py of yolov5 deepsort
- I have set a threshold value where the algorithm will cast a bounding box on a car if it doest go below it and thus will prevent duplicate counting
- I have tuned the parameters like accuracy confidence and threshold for the bounding boxes so that i get the correct labels and bounding box for tracking
- I have prepared the custom dataset in such a way that the cars that can be seen at the edge of the screen are also counted as they are slightly visible

# Thus i have tracked overall 104 cars including the cars that are seen slightly at the edge of the screen
