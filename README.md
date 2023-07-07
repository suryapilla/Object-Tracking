# Orientation-Tracking-and-Panoramic-image-generation

## Objective:
Implement a projected gradient descent algorithm to track the 3-D orientation of a rotating body using
readings from an inertial measurement unit (IMU). Using your orientation estimates, generate a panoramic
image by stitching camera images obtained by the rotating body

## Results of Roll, Pitch and Yaw before and after optimization
![Alt Text](https://raw.githubusercontent.com/suryapilla/Object-Tracking/main/figures/data2/roll2.png)

![Alt Text](https://raw.githubusercontent.com/suryapilla/Object-Tracking/main/figures/data2/Pitch2.png)

![Alt Text](https://raw.githubusercontent.com/suryapilla/Object-Tracking/main/figures/data2/yaw2.png)

## Results of panoramic stitching:
![Alt Text](https://raw.githubusercontent.com/suryapilla/Object-Tracking/main/figures/panStiching/9.png)

## Code:

1. Install the requirement files in new virtual environmnet: 
```
conda create --name env_ObjTrack
conda activate env_ObjTrack
git clone https://github.com/suryapilla/Object-Tracking.git
pip install requirements.txt
```
2. utilsCam.py and utils.py files have all the relevant functions required for the main function

3. setup the path as per the config.yml file in config directory

4. For training run the main function by giving the correct path to the data folder
```
python main.py
```

5. There are 3 sections in the main.py script:

	- Object tracking part

	- Plotting the roll, pitch and yaw for VICON, Unoptimized and Optimized data
	
	- Panorama generation
	
6. For testing run testMain.py script, with correct test data directory in path
```
python testMain.py
```

7. This is for testing data where VICON data is not available, the flow is similar to the main.py
	
	- Object tracking part
	
	- Plotting the roll, pitch and yaw for Unoptimized and Optimized data
	
	- Panorama generation
 
