# Plant Disease Detection App Demo
This repository is only to show the working of the plant disease detection project. All the development codes are kept confidential.

### Project Description
This project in collaboration with University of Florida is developed for quick, cheap and reliable on-site disease detection in plants. Since lab testing is not feasible in remote locations, this type of application is essential as a first stage diagnosis.  
User simply attaches a detachable *microscopic*(30x magnification) lens to their smartphone and captures images of the leaves/fruits of the plant. Prior research conducted at the *macroscopic* level has resulted in high validation metrics, but low detection capabilities in the field.  
17 biotic and abiotic diseases are taken into consideration of *tomato* plant because of their high economic importance.  
Multiple models are trained and work in a chained fashion to determine the final output. Models can predict whether the provided image is of the upper or lower part of the leaf*(Important for tomatoes since diseases are more prominent on the upper part)*. Models can also reject the image if it is blurry.

### Results and Recognitions
* 94% testing accuracy with 98% F1-score was achieved on test data obtained from fields in Florida. Further field validation is currently going on to expand the demographics.
* Received grants worth $25,000 from Microsoft AI for Earth.

### WebApp
WebApp is built using Streamlit. If identified, outputs are prediction confidence for each class received from the model output. A feedback mode is provided designed for pathologists to complete the data flywheel and the images are stored based on the received feedback in an Azure Blob Storage.

![](https://github.com/mubin-statlogic/Demo-Plant-Disease-Detection.git/feedback_demo.mp4)