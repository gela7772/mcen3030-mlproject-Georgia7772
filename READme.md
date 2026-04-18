## Deliverable 1 

Initial Prompt: I would like to do a machine learning project where the goal is to predict how old a snail is based on physical measurements. I have a spreadsheet with columns ‘sex’, ‘length’, ‘diameter’,
‘height’, 'whole weight', 'shucked weight', 'viscera weight', 'shell weight', and ‘rings’. There are approximately 4177 rows. I will ask for matlab code soon, but first: 
Can we talk about the best way to model this data set?

## Deliverable 2 

Due to the fact that we are measuring and tracking biological data - snails, diameter, weight, etc. - our dataset is not going to be perfect and should vary a lot.
I talked with my LLM about using two different methods: Gradient Boosting and Random Forest. In the end, Random Forest was the method that was recommended for many reasons. 
First, we will be hardcoding values for the sex of each snail, as they are not numbers. Second, Random Forest accommodates data that is nonlinear - most likely where we will
find ourselves. Third, his method is also good at finding correlations between variables, such as diameter and length, and making assumptions based on that knowledge. 
Finally, Random Forest is better for different types of data - this is useful in our case so we can combine length, weight, and sex in one dataset. Random Forest averages
several results in the end so we have a quicker baseline of our data analysis. In comparison, Gradient Boosting iterates and improves our results as we go. It is great for 
datasets with low variance in measurements requiring highly accurate analysis with low bias, however, as we are working with biological measurements, we will likely have more
variance in our dataset. Overall, Random Forest proves itself to be the better method for analyzing our data.  

## Deliverable 3

![Confusion_Matrix_from_Iteration_1](Confusion_Matrix_1.png)

Initially, my LLM disliked the idea of using a confusion matrix. With creating the confusion matrix, 
we have to eliminate pieces of the data so the snails will fit into age categories. The matrix generated 
in my initial iteration of code is in a strange configuration that is confusing to interpret. 
I will have it rearrange the order of the matrix. However, this matrix is showing us that each blue bin 
is where the Random Tree method predicted the correct number in the category. Each orange box is where
the method predicted the wrong number. The depth of the color helps to visualize the quantity of snails
in each bin. 

## Deliverable 4







