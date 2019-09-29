# **Problem Statement :**
- ### `To extract  the license number of a car from the plate.`

# **Softwares and Technology used :**
- OpenCV 3
- Python 3
- Tensor Flow

# Flow

The ALPR system consists of following steps:-
  - Preprocessing.
  - Character segmentation.
  - Character recognition.

# **Approach used and Implemented :**

- ## 1) Loading the Image :
- ## 2) PreProcess the input image :
  - This step in done in the Preprocess.py file.
	As most of the opencv function require the input iamge to be in the grayscale and greyscale images are easy for computation so we convert the input image to greyscale.
- ## 3) Plate detection :
  - We trained a model using tensor framework to detect plate in an image.
- ## 4) Character Segmentation :
	- This phase is done in the DetectChar.py file.
	Here we start with each possible plates.
	We crop the plate from input image and resize it to 1.6 times height, 1.6 times width. The we again apply the preprocessing operations on the plate image.
- ## Character recognition :
	- This part is done in the train_detect.py file.
