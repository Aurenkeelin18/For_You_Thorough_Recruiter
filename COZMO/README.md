![](04_Documentation/Images/COZMO_Title.png)
<br>
Interested in learning more about Cozmo? Visit the [developper website](https://developer.anki.com/)   and the [Cozmo by Digital Dream Lab website](https://www.digitaldreamlabs.com/pages/cozmo)
<br>

# PLAN

![.](04_Documentation/Images/plan.png)
<br>

# SAMPLING STRATEGY

![](04_Documentation/Images/samplingstrategy.png)

<br>
Watch the sampling video: [nnn]https://user-images.githubusercontent.com/68656802/162626900-25fed48a-d4df-487f-8ee3-277e0460e1dc.mp4


# IMAGE PREPARATION AND SELECTION

![](04_Documentation/Images/imageselection.png)

# MODEL AND METRICS
The model is a keras sequential model, optimized by root mean square propagation (rmsprop) with a categorical cross-entropy loss function, and a batch size of 30. The model without callbacks reached an accuracy of 83% after 100 epochs while the model with the “ best callbacks” reached an accuracy of 77% after 100 epochs. The accuracy and loss curves suggest that the validation images are not representative and that both training and validation images should be shuffled. After the shuffle the model reaches accuracy of 99.8%. The validation accuracy curve is better than the training curve because the model uses a dropout layer (50%).
![](04_Documentation/Images/Metrics.png)
![](04_Documentation/Images/Modelshufflesmall.png)



# MODEL APPLICATION
Cozmo looks at an item and collects new images. The images are normalized and sent to the model. The model classifies the images and provides an answer. Cozmo says what it is and giggles when he identifies a known letter. 
See Cozmo identifies the letters.
<br>
Watch the reading video: https://user-images.githubusercontent.com/68656802/162626956-638d79b7-8939-4e4f-9ec6-fc4a1f6990a1.mp4


# CONCLUSION
Simple Convolutional Neural Networks are relatively easy to build and make very powerful models for image classification and object detection.
<br>
The sequential model used in this project has good accuracy (>80%) but the accuracy curve shows that there is a need to shuffle the images between training and validation. Adding more images would be also beneficial.
<br>
As of now Cozmo just says the prediction of the model or “I don’t know this one” if the class is not known from the model yet. A confidence level using the model uncertainty and data uncertainty could be added to the program to prevent Cozmo from saying a wrong prediction.
