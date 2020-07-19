# Fashion-MNIST

# Basic classification: Classify images of clothing

In this notebook we train a neural network to classify the images of clothings.

Data for this project were provided by DAC club of my institue. Data can also be found online.

Problem is as follows--

Given a grayscale image(28 X 28), build a model to determine which article of clothing it represents.

**Description--**

Each image is 28 pixels in height and 28 pixels in width, for a total of 784 pixels
in total. Each pixel has a single pixel-value associated with it, indicating the lightness or
darkness of that pixel, with higher numbers meaning darker. This pixel-value is an
integer between 0 and 255. The training data set has 785 columns. The first column
consists of the class labels and represents the article of clothing. The rest of the
columns contain the pixel-values of the associated image.
● To locate a pixel on the image, suppose that we have decomposed x as x = i * 28
+ j, where i and j are integers between 0 and 27. The pixel is located on row i and
column j of a 28 x 28 matrix.
● For example, pixel31 indicates the pixel that is in the fourth column from the left,
and the second row from the top, as in the ascii-diagram below.

**Labels--**

Each training and test example is assigned to one of the following labels:
● 0 T-shirt/top
● 1 Trouser
● 2 Pullover
● 3 Dress
● 4 Coat
● 5 Sandal
● 6 Shirt
● 7 Sneaker
● 8 Bag
● 9 Ankle boot

Summary:
1. Each row is a separate image
2. Column 1 is the class label.
3. Remaining columns are pixel numbers (784 total).
4. Each value is the darkness of the pixel (1 to 255)



# Model
Here we used keras Sequential model to train a neural network.

First, we train on less data and use remaining for validation purpose, later we train the same model on full dataset and uses this new model to make predictions on test datas.
Here, we got more than 94% accuracy on training set while near about 93% accuracy on test dataset.
