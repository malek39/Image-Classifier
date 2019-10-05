# Image-Classifier
In this project, you'll build a Python application that can train an image classifier on a dataset, then predict new images using the trained model.
In this lab you will use a created image classifier to identify dog breeds. We ask you to focus on Python and not on the actual classifier. (We will focus on building a classifier ourselves in other program).

Description:
Your city is hosting a citywide dog show and you have volunteered to help the organizing committee with contestant registration. Every participant that registers must submit an image of their dog along with biographical information about their dog. The registration system tags the images based upon the biographical information.

Some people are planning on registering pets that aren’t actual dogs

You need to use a newly developed Python classifier to make sure the participants are dogs.
Lab Goals

Tasks:

    Using your Python skills, you will determine which image classification algorithm works the "best" on classifying images as "dogs" or "not dogs".

    Additionally, you want to determine how well the "best" classification algorithm works on correctly identifying a dog's breed. Fortunately, the registration system will tag each photo with the registered dog's breed (as entered by the participant). Your program will only need to compare the photo's filename (which will include the breed) to the breed that the classification algorithm returns. For images where the breed differs, other volunteers will call and verify a dog's breed.

    Finally with computational tasks, there is often a trade-off between accuracy and runtime. The more accurate an algorithm, the higher the likelihood that it will take more time and use more computational resources to run. To better prepare you for discussing this and exploring the "best" option when solving a problem computationally, we would like you to time how long each algorithm takes to solve the classification problem.

    If you have questions or otherwise run into issues while working on this lesson, please check our FAQ here.

Important Notes:

For this image classification task you will be using an image classification application using a deep learning model called a convolutional neural network (often abbreviated as CNN). CNNs work particularly well for detecting features in images like colors, textures, and edges; then using these features to identify objects in the images. You'll use a CNN that has already learned the features from a giant dataset of 1.2 million images called ImageNet. There are different types of CNNs that have different structures (architectures) that work better or worse depending on your criteria. With this lab you'll explore the three different architectures (AlexNet, VGG, and ResNet) and determine which is best for your application.

We have provided you with a classifier function in classifier.py that will allow you to use these CNNs to classify your images. The test_classifier.py file contains an example program that demonstrates how to use the classifier function. For this lab, you will be focusing on using your Python skills to complete these tasks using the classifier function; in the Neural Networks lesson you will be learning more about how these algorithms work.

Understand that certain breeds of dog look very similar and any of these algorithms' ability to distinguish between two breeds of dog is only as good as the dataset (ImageNet) and the algorithm. Meaning that the more images of two similar looking dog breeds that the algorithm has learned from, the more likely the algorithm will be able to distinguish between those two breeds. This is also true for you, the more images of two similar dog breeds you see in knowing their true identification; the better you will become on distinguishing between those two breeds of dog. We have found the following breeds to look very similar: Great Pyrenees and Kuvasz, German Shepherd and Malinois, Beagle and Walker Hound, and others.

Finally, note that some dog breeds, like Greyhound and Australian Shepherd, are not breeds of dog that have images in ImageNet. This means the algorithms would never be able to correctly classify those breeds of dog because they have never seen them before. The best the algorithms can do is to classify those images as some similar looking breed of dog that does exist in ImageNet. For the images you will be testing the algorithms on, only dog breeds that exist in ImageNet will be used.


Principle Objectives

    Correctly identify which pet images are of dogs (even if breed is misclassified) and which pet images aren't of dogs.
     
    Correctly classify the breed of dog, for the images that are of dogs.
     
    Determine which CNN model architecture (ResNet, AlexNet, or VGG), "best" achieve the objectives _1_ and _2_.
     
    Consider the time resources required to best achieve objectives _1_ and _2_, and determine if an alternative solution would have given a "good enough" result, given the amount of time each of the algorithms takes to run.
