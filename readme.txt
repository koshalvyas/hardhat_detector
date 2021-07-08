data source: https://www.kaggle.com/andrewmvd/hard-hat-detection/discussion/186098

Data-preprocess:
Used facenet for face detection
cropped faces from images with helmet and saved in one folder
cropped faces from images without helmet and saved in another folder
Used data augmentation to add more images

HardHat Detector:
Trained a single layer cnn on top of pretrained mobilenetv2 for detecting faces with helmet.
feed video from webcam to detect hardhat

How to run.
1. Dake two directories one for people with hard hat and other without hard hats
2. Run data pre_processor
	a. use data-preprocess file to detectect face with helmet and save it one directory
	b. do same for people without hardhats
3. Run helmet detector with paths of two directories
