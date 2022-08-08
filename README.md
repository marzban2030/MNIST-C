# MNIST-C
Fast handwritten digit recognition by using MNIST dataset in full C++ code

The C++ programming language, Fastest processing and lowest memory usage in world of computer programing languages. It is also mother of other programing languages. It load MNIST dataset into less than 10MB of RAM and test dataset images in few seconds. Let's go!

Minimum hardware requirements: (tested)

Intel pentium III CPU

64MB RAM

100MB free disk space


Requirements:

"mnist_train.csv" and "mnist_test.csv" files from Google.

Installed "Clang" compiler.


Running instruction guide:

1- Clone this repository to your working directory.

2- Go to cloned repository folder.

3- Unzip "UnzipMe.zip" file which is in the repository folder or download required CSV files from Google to repository folder.

4- Compile "test.cpp" code and build binary file with "clang++" command.

5- Execute binary file.

Doing above instructions in my VPS:
![Image1](https://github.com/marzban2030/MNIST-C/raw/main/test0101.jpg)

96% accuracy for handwritten digit recognition by this C++ code. Actually this C++ code compare each BW test image pixels with all of BW train images pixels by means of bitwise operation after turning each train and test image to a 784 bit binary value, And find difference between these; Then choose that train image which has minimum difference with desired test image.

Speed of images testing per second = CPU single core speed in HZ / (784bit × 60000 train images)

For example a 233MHZ Pentium II processor can test 5 images per second = 233,000,000/(784×60,000) by this C++ code. It means this CPU recognize a handwritten digit in 0.2 second. This C++ code can be compiled and executed in an old computer with 80386 microprocessor but todays AI digits recognition programs/modules such as Google TensorFlow need very strong hardwares (Corei7 CPU with 4GB RAM and strong GPU).

At future versions of this C++ code, I will define more effective comparison function to taking 99% accuracy at least. I will focus on maximum speed and accuracy, And less memory usage.

This project can be developed easily to recognize everything in computers, automotive cars, robots, drones, space telescopes and so on.
