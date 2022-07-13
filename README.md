# Read_Hand

## Sign Language and Static-Gesture Recognition
Gesture recognition is an open problem in the area of machine vision, a field of computer science that enables systems to emulate human vision. Gesture recognition has many applications in improving human-computer interaction, and one of them is in the field of Sign Language Translation, wherein a video sequence of symbolic hand gestures is translated into natural language.
<br>
## Dataset
The dataset format is patterned to match closely with the classic MNIST. Each training and test case represents a label (0-25) as a one-to-one map for each alphabetic letter A-Z (and no cases for 9=J or 25=Z because of gesture motions). The __training data__ (27,455 cases) and __test data__ (7172 cases) are approximately half the size of the standard MNIST but otherwise similar with a header row of label, pixel1, pixel2....pixel784 which represent a single 28x28 pixel image with grayscale values between 0-255. 
<br>
## Data Preprocessing
As the dataset has already given csv values for images, we don't need to do much preprocessing. If dataset of image was in raw format, we have to convert them in csv format arrays before doing any of the further operations. Still we perform following steps:

- Seperate features(784 pixel columns) and output(result label)
- Reshape the features
- One Hot Encoding on result 

## Model

We will use Keras to build the simple CNN(Convolutional Neural Network).
There are total 7 layers in the CNN:

1. 1st Convolutional Layer with `relu`
2. 1st Max Pooling 
3. 2nd Convolutional Layer with `relu`
4. 2nd Max Pooling
5. Flattening
6. First Full Layer with `relu`
7. Output Layer with `sigmoid`


## Technologies Used 
* Deep Learning
* Speech Recognition
* CNN-Keras
* Python 
* Win32com
* Image Processing
* Image Recognition
* Docx

## Challenges
The major challenge was to make this project light and not dependent on internet. So we had to use libraries which used minimum internet in order to carry out the task.  We could not use any APIs as they'd require the use of internet. Secondly creating sign language transcripts was rather difficult because there wasn't any existing font for it and the ones which resembled closely weren't legible. So we had to scout images which were clear and could be used and yet maintain uniformity. 
So we had to scout images which were clear and could be used and yet maintain uniformity. The next challenge was the sign to text converter.We had to design a model what was fast and accurate to differentiate between words and spaces and we somehow did a decent job at it. Since it's already a challenge to create a level playing ground for those who are differently abled, we believe we did give a great start to the initiative to bring about some attention towards this as this might be the new normal for a while now.

## Key Features of Program
* It converts ASL SIGN hand gestures to English TEXT dynamically.
* It converts Speech to Braille script proactively.
* It converts English TEXT to SIGN hand gestures.


## Results
- Training Set Accuracy: `96.06 %`
