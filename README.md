# Vision-and-Language Driving: A Benchmark for Long-horizon Human-instructed Autonomous Driving


We introduces a novel task, **Vision-and-Language Driving (VLD)**, aiming to enable vehicles to follow long-horizon human natural-language instructions to autonomously navigate in traffic environments. We also build a dataset (**VLD dataset**) for the VLD task and proposed a baseline approach based on fine-tuning Qwen2-VL.




## Data Collection and process


We use CARLA 0.9.15 to collect data with the Leaderboard 2.0 framework in Town 12. We design driving routes by configuring starting points, waypoints, and end points. 

The vehicle is equipped with multiple sensors: four RGB cameras, four semantic cameras, four depth cameras, and one LiDAR. Our sensor placement is developed from the [DriveLM](https://github.com/OpenDriveLab/DriveLM) placement scheme, which is shown in the figure below. The specifications of the sensors is displayed in the table below.

<div align=center>
<img src="https://github.com/lab-sun/VLD/blob/main/pics/sensors.png" width="700px"/>
</div>







## VLD Dataset Detail and Download

The VLD dataset is constructed based on the CARLA simulator, which contains RGB images, Graph-of-Thought (GoT) format VQAs, Chain-of-Thought (CoT) format VQAs, and human language instrcutions for the corresponding driving routes. 

**The VLD dataset contains $260$ long-horizon human-language instructions, and around $1.5$ million VQAs for $44,999$ frames**.

You can download the full VLD dataset from [here](https://144.214.80.11:5001/sharing/7acEIXQEE) ``(Please use the password provided in the manuscript to access the download page and unzip the zip files.)`` and download the preprocessed raw data [here](https://144.214.80.11:5001/sharing/yU1G0LiAF) ``(Please use the password provided in the manuscript to access the download page and unzip the zip files.)`` , which was used to generate the full VLD dataset. The preprocessed raw data data contains additional information collected from the CARLA simulator, so that you can also generate further interesting datasets based on this material to suit your own requirements. 

We will subsequently release all collected data (i.e., raw data) collected from the CARLA simulator.


The full dataset is very large, especially the JSON files that store the VQAs. We recommend opening them with VSCode. If you'd like to get a quick understanding of our dataset, we provide the complete content of a single route from the VLD dataset, which you can download [here](https://144.214.80.11:5001/sharing/HvcjGQb1U) ``(Please use the password provided in the manuscript to access the download page and unzip the zip files)``.


## Sample Driving Route and Instructions 

The following video is an RGB recording of a vehicle's driving route from the VLD dataset, with the instruction being ``Go straight along the current road, turn left at the T-junction after passing a blue-purple kiosk, then go straight, turn right at the T-junction after passing a white plastic table, then go straight, turn left at the T-junction at the end of the road, then go straight, turn left at the crossroads after passing a Coca-Cola vending machine, then go straight, turn right at the T-junction at the end of the road, then go straight and stop near the mailbox on the right side of the road. ``

https://github.com/lab-sun/VLD/assets/112605189/521228503-c61c8795-1904-4c27-a0fc-a551b8827784


For more detailed information, please refer to the content within the paper. 



## Sample Results


https://github.com/lab-sun/VLD/assets/112605189/521228946-cd013c85-33a1-40c5-80a8-436d84045b09

# Acknowledgement

Thanks for [DriveLM](https://github.com/OpenDriveLab/DriveLM).


