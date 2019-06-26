I'm using python 3.7
To run the project run the command

	$ jupyter notebook

and browse into the folder using your web browser

1. Whenever the  training data is decreased, the accuracy also decreases. 
Furthermore, the depth of the tree generated and the number of nodes also decrease when the 
training data decreases from 80% to 10%. We observe the gini value gradually decrease although
not smoothly. According to wiki, Gini is used by the CART (classification and regression tree) 
algorithm for classification trees, Gini impurity is a measure of how often a randomly chosen 
element from the set would be incorrectly labeled if it was randomly labeled according to the 
distribution of labels in the subset. This is somehow different from the entropy function used in 
class where entropy is purely used as a measure of uncertaininty.

I notice that 2 or 3 levels are a good indicator of the benigness or malignancy of a sample.
For instance 
	
	Uniformity_Thickness <= 3.5 && Bare_Nuclie < 3.5 && Clump_Thickness <= 6.5

	Then its most likely that the tumor is benign (98.6%)

This tells us that we can easily apply prunning at this stage.

2. Accuracy: 0.94 (+/- 0.04)

3. Accuracy: 97.70%
   Accuracy: 98.85%
   Accuracy: 97.70%
   Accuracy: 90.80%
   Accuracy: 94.25%
   Mean Accuracy: 95.86%
   Interval: +/- (1.87)%