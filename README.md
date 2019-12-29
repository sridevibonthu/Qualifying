# Qualifying Assignment

I have executed and understood david net.
To complete the assignment, first i tried all the pretrained models vgg, resnet and inception.


In my model i experimented in several ways. Used Data Augmentation (cutout also) and tried all the three variations of CLR and understood about LR range test. I am posting accuracies of only two models here.


Through EDA, I understood that there are some problem in annotations (i.e., in data). I am submitting those models which are trained on the supplied data.


Thanks alot for giving this opportunity to learn and explore this different kind of Multilabel classification. Many multilabel classifications, I have seen are using Binarycrossentropy.




## [Model 1](https://github.com/sridevibonthu/Qualifying/blob/master/Model_with_separable_conv.ipynb) 
* val_gender_output_acc  --  0.8504464285714286
* val_image_quality_output_acc  --  0.5714285714285714
* val_age_output_acc  --  0.41443452380952384
* val_weight_output_acc  --  0.6428571428571429
* val_bag_output_acc  --  0.6499255952380952
* val_footwear_output_acc  --  0.6648065476190477
* val_pose_output_acc  --  0.7927827380952381
* val_emotion_output_acc  --  0.7053571428571429


## [Model 2](https://github.com/sridevibonthu/Qualifying/blob/master/modularized.ipynb)
* val_gender_output_acc  --  0.8566468253968254
* val_image_quality_output_acc  --  0.5248015873015873
* val_age_output_acc  --  0.3566468253968254
* val_weight_output_acc  --  0.5942460317460317
* val_bag_output_acc  --  0.6483134920634921
* val_footwear_output_acc  --  0.6369047619047619
* val_pose_output_acc  --  0.8139880952380952
* val_emotion_output_acc  --  0.6944444444444444

To come out of OutOfMemory error, I have used Separable Convolution Layers and reduced parameters

In Model 2, CLR and cutout are used.
