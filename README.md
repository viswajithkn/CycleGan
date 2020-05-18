# CycleGan
CycleGan for Season Transfer
A GAN - short for Generative Adversarial Networks - have been used in a wide array of applications ranging from fashion, 
to face aging, object visualizations and art transfer to name a few. CycleGan is one such network which can be used for 
unpaired image translations. 
Image translation typically involves paired images. One in Domain A and one in Domain B for each image. Now what happens 
if we do not have such paired images? What if we have a set of photographs of Yosemite during the summer and another 
random bunch of photographs of Yosemite during the winter? Is it possible to translate the summer pics to winter and vice versa?

The link to the original author's work and results are here. The model was trained for 100 epochs with random sampling
of the training images. The interesting aspect of the results were that the testing results on the winter to summer 
translation were not complete in quiet a few of the testing images. 
May be more training would improve the results of the second generator in the model. The next step in this direction 
would be to train the model for the next 100 epochs with a training decay as mentioned in the paper. I would also love 
to explore a system where the learning rate on the discriminator is slightly lower in comparison to that of the generator to 
see if this facilitates better conversion from the generators.
