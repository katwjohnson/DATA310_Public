# Response for Class on 7/20

## Cats and Dog Classifier

## Question 1: Which optimizer have you selected, and how might it compare to other possible choices?

### Answer:
  For the cat vs. dog model the optimizer I used was RMSprop. RMSprop, root mean square prop, was selected over other optimizers because of its ability to keep adjusting the average of the squared gradients for each weight then dividing the gradient by the square root of the mean square. By using the moving average, the learning rate is able to be adapted. Additionally, RMSprop works better for larger datasets than other optimizers such as Rprop and Adam.
  [Link](https://towardsdatascience.com/understanding-rmsprop-faster-neural-network-learning-62e116fcf29a)
  
## Question 2: Describe your selected loss function and it’s implementation.  How is it effectively penalizing bad predictions?

### Answer:
  I used the binary cross-entropy loss function, because the classification is binary (cat or dog). The loss function penalizes bad predictions based on the prediction’s probability. In other words, if the probability between an image and its actual label is low (like .015) then the loss has to be large. However, if the probability between the image and the actual label is 1.0 or close to 1.0 then the loss has to be zero or close to zero.
  [Link](https://towardsdatascience.com/understanding-binary-cross-entropy-log-loss-a-visual-explanation-a3ac6025181a)
  
## Question 3: What is the purpose of the metric= argument in your model.compile() function?

### Answer:
  A metric function is used to determine how well a model is performing. There are different types of metrics depending on how someone would want to evaluate the performance of their model. 
  [Link](https://keras.io/api/metrics/)

## Question 4: Plot the accuracy and loss results for both the training and test datasets.  Include these in your response.  Assess the model and describe how good you think it performed.

### Answer: 
  The model performed okay, with that being said it is still clearly overfit. Between the 14th epoch and the 15th epoch the validation accuracy went from 0.8167 to 0.7913. Then looking at the graphs the loss validation goes up and down a couple of times, but especially around the 9th epoch.
  ![](Resp_7_20_1.png)

## Question 5: Use the model to predict 3 dog images and 3 cat images.  Upload you images and the prediction.  How did your model perform in practice?  Do you have any ideas of how to improve the model’s performance?

### Answer:
  When I uploaded my 3 cat and 3 dog images it only misclassified one image. The model correctly identified all of the dog images. Then with the cat images it correctly labeled 2 images, including the one of Taylor Swift from the movie Cats, but it did mislabel the image of the cat dressed up in sunglasses and a bowtie. Considering the overfitting the model performed better than I thought it would with my images. I would run fewer epochs and probably adjust the learning rate.
  
  ### Cat Images
  
  ### Correctly Labeled
  
  ![](Cat1.jpg)
  
  ![](Cat4.jpg)
  
  ### Incorrectly Labeled
  
  ![](Cat3.jpg)
  
  ### Dog Images
  
  ### Correctly Labeled
  
  ![](Dog1.jpg)
  
  ![](Dog2.jpg)
  
  ![](Dog3.jpg)
  
  
  
  
