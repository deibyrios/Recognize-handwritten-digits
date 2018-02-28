# Recognize-handwritten-digits
Recognize handwritten digits using "nearest neighbor" classifier, which is incredibly simple and effective for this type of problems. Achieved 96.91% precision rate after testing with 10,000 test digits!

 What I found most amazing was that manually programming the algorithm by myself to return the ‘predicted’ digit on the 10,000 new test user inputs, only required me to write 2 lines of code in Python and the algorithm ran just a few seconds in my laptop. 

 As ‘training’ data, I used 60,000 previously prepared and correctly classified examples that my algorithm used to "learn" how to correctly classify future user inputs. The images were centered and standardized to the same size, then converted into a vector (straightforward technique commonly used to represent images in a way that can be understood by the machine).

 For a single new user input, we apply the same transformation from image to vector and then pass it to the algorithm. The algorithm then computes the distance between the new input vector and all 60,000 vectors that it uses as ‘training’ examples and returns the digit associated to the training example whose distance to the new user input is the minimum distance among all training examples, that’s it!
