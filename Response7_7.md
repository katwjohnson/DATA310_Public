# Response for Class on 7/7

## Question 1:
### In Laurence Maroney’s video, What is ML, he compares traditional programming with machine learning and argues that the main difference between the two is a reorientation of the rules, data and answers.  According to Maroney, what is the difference between traditional programming and machine learning?

### Answer:
  In traditional programming the inputs are both data and a set of rules. Based on those inputs, answers can be produced. During the input phase the programmer is expected to understand and correctly codify the rules so the program can produce accurate answers or labels. In machine learning the inputs and outputs are shifted. Machine learning allows the rules to be produced by matching the patterns provided through data to be matched with the answers or labels. In other words, the data and answers are the inputs while the rules are what is inferred or produced.
  
## Question 2:
### With the first basic script that Maroney used to predict a value output from the model he estimated (he initially started with 10 that predicted ~31.  Modify the predict function to produce the output for the value 7.  Do this twice and provide both answers.  Are they the same?  Are they different?  Why is this so?

### Answer:
  The two answers that I got were 40.00138 and the other was 40.00141. The two answers are different because, the model that we are running is trained on only six points of data. The features (X’s) relative to the targets (Y’s) for the six points do show a linear relationship; however, if you increase the quantity of points significantly there is no guarantee that will remain true for other points. While the neural network will take the linear relationship for these six points into account, it will not predict the same exact target answer for a desired feature value because other data points could be skewed in an unknown number of different directions.
  
## Question 3:
### Using the script you produced to predict housing price, take the provided six houses and train a neural net model that estimates the relationship between them.  Based on this model, which of the six homes present a good deal?  Which one is the worst deal?  Justify your answer.

### Answer:
  After fitting the model, it appears that the worse value relative to bedrooms is the Church house while the best values are Hudgins and Holly houses. An aspect of this model that is extremely limiting is that the only variable it takes into account is bedrooms. There are many other variables such as location, amenities, age, history, square footage, etc. that could be taken into account in order to produce a more realistic estimated price.
  
