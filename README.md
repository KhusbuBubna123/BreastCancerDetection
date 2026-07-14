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

	The results of classification obtained were as follows:
	
	SVC(Support Vector Classifier)-----Accuracy(0.97)----Recall(0.97)----f1_score(0.96)
	Grid SVC(Using Grid Search)-------Accuracy(0.97)    Recall(0.97)  f1_score(0.96)

	Decision Tree Classifier    Accuracy(0.93)   REcall(0.875)   f1_score(0.923)
	Using Grid Search Decision Tree Classifier  Accuracy(0.93)  Recall(0.9069)  f1_score(0.9069)

	Random Forest Classifier   Accuracy(0.96)  Recall(0.975)  f1_score(0.952)
	Gradient Boosting          Accuracy(0.96) Recall(0.9756)   f1_score(0.9523)
	XGBoost                    Accuracy(0.964)  Recall(0.9756)  f1_score(0.9523)

	K Nearest Neighbors Classifier  Accuracy(0.9649)  Recall(0.95348)  f1_score(0.95348)

	Linear Regression R2 score(0.89722)  Mean Squred Error(0.032489) Root Mean Squared Error(0.18025) Mean Absolute Error(0.12567)
