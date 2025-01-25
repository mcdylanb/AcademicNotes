### Thesis Candidate
- Drone that helps Civil on Road Con
	- we will use 5 directional drone, maybe 6
	- using ai image recognition to identify inventory
		- like signage
	- follows through center line
	- able to measure the width
	- able to measure distance 
		- per block 10m
		- and per 1km 
	- We might have to create a study of accuracy difference for alternative wheel 
	- Possible Issues
		- the accuracy of measurement using image
			- https://inria.hal.science/inria-00548411/file/brand94accuracy_1.pdf
			- Suggestions in increasing distance measuring using drones
				- High-Precision GPS: Equip drones with Real-Time Kinematic (RTK) or Post-Processing Kinematic (PPK) GPS systems. These systems provide centimeter-level accuracy by using corrections from ground-based reference stations.
					- COMMENT: must be costly more devices needed
    
				- Lidar Integration: Pair the drone with a Lidar sensor. Lidar creates high-resolution 3D maps of the terrain, allowing for accurate distance measurements even on uneven road surfaces.
					- we will have to measure compare using the wheel
					- then compare with image recognition
				    
				- Aerial Photogrammetry: Use the drone to capture overlapping aerial images and generate detailed orthomosaic maps. These can be processed with software to calculate distances accurately.
				    
				- Automated Flight Paths: Plan precise, repeatable flight paths for the drone using mapping software. This ensures consistency in data collection across different road segments.
				    
				- Georeferenced Maps: Combine the drone data with existing high-precision georeferenced maps to cross-verify and refine measurements.
		- cracks depth
			- which we can allow detection from drone and notify engineers for manual checking