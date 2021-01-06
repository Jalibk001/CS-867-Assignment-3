# CS-867-Assignment-3

In this assignment, a VGG-16 network has been used for predicting the natural images, belonging to classes buildings, forests, glaciers, mountain, sea and street.


Given below is the model of VGG-16 used

![VGG-16](https://drive.google.com/uc?id=1mcX1ikWBp06wcMF5xQJXGB1_7mA-McMm)

In this case, firstly the model entire model was trained, with 50 epochs, but considering the training results, accuracy was not increasing once the 20th epcoh crossed, so therefore the model was set to train for 20 epochs only, and the validation accuracy was found to be 92% whereas the testing accuracy was found to be 89.6%

Next time the model was trained using transfer learning with image augmentation, the shear range appplied was 0.2 and the zoom range applied was 0.2 and the images were flipped as well, so as to allow better augmentation, next considering the large amount of data, 7 layers were trained out of 22 and the rest of the 15 layers were kept frozen and the training results are depicted below for the described model

![VGG-16](https://drive.google.com/uc?id=1EMhcQ_yZEpUcjoCj3jPQ1o1n2lCaD84d)


The validation accuracy is found to be 91% whereas the testing accuracy was 90.8% 


For both the above models, the weights have been stored

The model in which transfer learning was not applied, the weights are saved in file name `vgg_non_transfer_weights.h5`, while the weights for the second trained model are stored in file `vgg_transfer_learning_weights.h5`
