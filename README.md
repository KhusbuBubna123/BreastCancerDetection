Breast cancer is the most common cancer amongst women in the world. It accounts for 25% of all cancer cases, and affected over 2.1 Million people in 2015 alone. It starts when cells in the breast begin to grow out of control. These cells usually form tumors that can be seen via X-ray or felt as lumps in the breast area.

The key challenges against it’s detection is how to classify tumors into malignant (cancerous) or benign(non cancerous). 

The features are:

	1)	id: Unique ID
	2)	diagnosis(Target):M (Malignant): Indicates a cancerous tumor. B (Benign): Indicates a non-cancerous tumor. 
	3)	radius_mean: Radius of Lobes
	4)	texture_mean: Mean of Surface Texture
	5)	perimeter_mean: Outer Perimeter of Lobes
	6)	area_mean: Mean Area of Lobes
	7)	smoothness_mean: Mean of Smoothness Levels
	8)	compactness_mean: Mean of Compactness
	9)	concavity_mean: Mean of Concavity
	10)	concave points_mean: Mean of Cocave Points
	11)	Symmmetry
	12)	Fractal dimension  ("coastline approximation" - 1)

	1)Radius: The mean of distances from the center of the cell nucleus to points on the perimeter.
	2)Texture: The standard deviation of gray-scale values, indicating the uniformity of cell shading.
	3)Perimeter: The total length of the boundary of the cell nuclei.
	4)Area: The total size of the area enclosed by the cell nucleus boundary.
	5)Smoothness: Local variations in radius lengths, measuring how jagged or smooth the cell outline is.
	6)Compactness: A shape descriptor calculated as \(\frac{\text{perimeter}^2}{\text{area}} - 1.0\).
	7)Concavity: The severity of indentations or concave portions along the boundary contour.
	8)Concave Points: The number of distinct concave portions found along the boundary contour.
	9)Symmetry: A measure of how symmetrical the shape of the cell nucleus is.
	10)Fractal Dimension: The "coastline approximation" that defines the geometric complexity or irregularity of the 	boundary.

	We are using different algorithms like K Nearest Neighbors Classifier,Logistic Regression,Support Vector 
	Machine Classifier,Decision Tree Classifier,Random Forest,etc to predict where a tumor is cancerous(Malignant) 
	or non-cancerous(Benign). We also used Linear Regression to predict the radius worst.
