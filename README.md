# Intermediate-Features-Fusion-based-CNN

The method determines the presence of subtitle in a video frame through intermediate features fusion-based Convolutional Neural Network (CNN) called the IFVSNet via partial transfer learning process on pre-trained
VGG13. The intermediate features from all the convolutional blocks of the CNN are fused by concatenation after each max-pooling layer. The features to be fused are of the same dimension. They are then flattened and
passed as an input to the subsequent fully connected layers, ending with the sigmoid layer. Binary cross-entropy is used as the objective function. The model is evaluated on the Film Videos Dataset (FiViD), which is
composed of video frames with and without subtitles in Arabic languages. We obtained an average accuracy of 98.83% which can be taken as an effective result. We have also conducted other experiments by fine-tuning 
the VGG13 model, another by using VGG13 as the features extractor and Long Short Term Memory (LSTM) as the classifier, and lastly, with a 3-layers CNN trained from scratch. It is observed that the performances of 
these three models are lower than the proposed methodology. The class-wise analysis of the proposed method has also demonstrated that the model is quite strong in distinguishing the classes present in the dataset and achieved a precision, recall, and F-score of above 98%.

<img src="https://github.com/Naosekpam/Intermediate-Features-Fusion-based-CNN/assets/46924277/d03d6bc8-f7c7-4f7a-a897-2587e3d83129" width="500" height="200">

# To cite :
Naosekpam, Veronica, and Nilkanta Sahu. "Ifvsnet: intermediate features fusion based cnn for video subtitles identification." 2022 IEEE 7th International conference for Convergence in Technology (I2CT). IEEE, 2022.

or 

```
@inproceedings{naosekpam2022ifvsnet,
  title={Ifvsnet: intermediate features fusion based cnn for video subtitles identification},
  author={Naosekpam, Veronica and Sahu, Nilkanta},
  booktitle={2022 IEEE 7th International conference for Convergence in Technology (I2CT)},
  pages={1--6},
  year={2022},
  organization={IEEE}
}
```
