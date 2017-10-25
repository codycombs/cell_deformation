# Instructions

The objective is to fit ellipses for every detection within every event that occurs in an OI video. The ellipses are then used to calculate the relevant physical parameters for the particle's trajectory, such as position, velocity, aspect ratio, etc.

1. Track the events.
	- This is done in the pore_stats/notebooks/oi_event_detection.ipynb notebook
2. Test the ellipse fitting parameters.
	- Use the 'test_ellipse_fit.ipynb' notebook
	- The ellipse fitting parameters will have to be changed in order to ensure a good fit
	- Usually the most important parameters to change are the Gaussian blur kernel and the intensity threshold
3. Fit ellipses
	- Use the 'fit_ellipses.ipynb' notebook
4. Filter ellipses
	- 'filter_ellipses.ipynb' notebook	
	- Filter the ellipses based on
		- Channel entrance/exit
		- Radius
		- Aspect ratio
		- Cavit y-position
