# Video_Classification

Different Categories of Sports Images(Cricket, Football and Swimming) were trained through transfer learning on Resnet101. 

For Video Classification the following steps were used-

1. Frames were extracted from every video using OpenCV
2. For every frame prediction was made from the trained model.
3. The maximum occuring class was predicted as the final prediction.
4. The output video was created with prediction over every frame.

## Motivation

Neural network architectures such as Long short-term memory (LSTMs) and Recurrent Neural Networks (RNNs) are suited for time series data but in some cases, they may be overkill. They are also resource-hungry and time-consuming when it comes to training over thousands of video files.

Instead, for some applications, all you may need is frame wise image classification as videos are mere combination of images.

## Tech/FrameWork Used

1. Python 3.7.3
2. Keras 2.2.4
3. OpenCV2

# Results

The Resnet101 model was trained for 30 epochs with initial learning rate of 0.01 and reduction on Plateau(minimum of 1e-05).

Over 90% accuracy was obtained on the validation data.

The predicted video had some class flickering but predicted correct class for substantial part of video.

# License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
