# Vision-and-Language Driving: A Benchmark for Long-horizon Human-instructed Autonomous Driving

We introduce a novel task, **Vision-and-Language Driving (VLD)**, aiming to enable vehicles to follow long-horizon human natural-language instructions to autonomously navigate in traffic environments.

**The paper of this dataset is under review.**

## Data Collection

This paper builds a dataset for the VLD task. We use CARLA 0.9.15 to collect data with the Leaderboard 2.0 framework in Town 12. We design driving routes by configuring starting points, waypoints, and end points.

The vehicle is equipped with multiple sensors: four RGB cameras, four semantic cameras, four depth cameras, and one LiDAR. Our sensor placement is developed from the [DriveLM](https://github.com/OpenDriveLab/DriveLM) placement scheme, which is shown in the figure below. The specifications of the sensors is displayed in the table below.

<div align=center>
<img src="https://github.com/lab-sun/VLD/blob/main/pics/sensors.png" width="700px"/>
</div>

## Downloads

``Please use the password provided in the manuscript to access the download pages and unzip the zip files.``

The full VLD dataset: [download link](https://nas.labsun.org/downloads/under_review/vld_dataset.php)

The preprocessed raw data: [download link](https://nas.labsun.org/downloads/under_review/vld_dataset_raw.php)

Note: The preprocessed raw data contains additional information collected from the CARLA simulator. You may develop your own datasets based on the raw materials for your own tasks. 

A mini sample data with a single route: [download link](https://nas.labsun.org/downloads/under_review/mini_sample_route_1263.php)

## Demonstrations

The following video is an RGB recording of a vehicle's driving route selected from the dataset, with the instruction:
``Go straight along the current road, turn left at the T-junction after passing a blue-purple kiosk, then go straight, turn right at the T-junction after passing a white plastic table, then go straight, turn left at the T-junction at the end of the road, then go straight, turn left at the crossroads after passing a Coca-Cola vending machine, then go straight, turn right at the T-junction at the end of the road, then go straight and stop near the mailbox on the right side of the road. ``

https://github.com/lab-sun/VLD/assets/112605189/521228503-c61c8795-1904-4c27-a0fc-a551b8827784

For more details, please refer to the paper. 

The prediction results:

https://github.com/lab-sun/VLD/assets/112605189/522255750-0d9a4694-9048-4864-aab7-ee8bfa6949e1

## Acknowledgement

[DriveLM](https://github.com/OpenDriveLab/DriveLM)

## Contact
[CityU Autonomous Systems Lab](https://labsun.org/)
[Prof. Yuxiang Sun](mailto:yx.sun@cityu.edu.hk)
