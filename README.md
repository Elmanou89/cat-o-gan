This project aims at generating artifical picture of my cat using a GAN. It's mostly for me to put the hands on such methods and was mostly based on the GAN tutorial of pytorch https://pytorch.org/tutorials/beginner/dcgan_faces_tutorial.html.
I first trained a model using a generic dataset found on kaggle: https://www.kaggle.com/crawford/cat-dataset
Here are some examples of inputs:
![Image of cat dataset](https://github.com/Elmanou89/cat-o-gan/blob/master/input_example/cats_generics.png)

I played a bit on the architecture but not so much. Increasing the input size of the random vector yields to much improved results:
![Image of output](https://github.com/Elmanou89/cat-o-gan/blob/master/output_example/generic_output.png)

Then I tried to "specialize" the network on pictures of my own cat:
![Image of my cat](https://github.com/Elmanou89/cat-o-gan/blob/master/input_example/mycat.png)

Which changed mostly the color of the cats in output, but not much the shape.
![Image of my cat](https://github.com/Elmanou89/cat-o-gan/blob/master/output_example/my_cat_output.png)
Overall I would like to train with other losses than the binary cross entropy, and I believe there is much room for improvement reagrding the training schedule.

The faces of the cat are not well defined at all, I'm not sure if playing on the architecture or loss could improve this, but also a much longer training (everything shown here was only trained for max 4-5 hours)




