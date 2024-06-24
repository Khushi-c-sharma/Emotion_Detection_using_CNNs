Emotion Detection using CNNs

Introduction :- 
This project aims to detect emotions from facial expressions using Convolutional Neural Networks (CNNs). I've leveraged data augmentation techniques and transfer learning with pre-trained models VGG16 and ResNet50 to enhance the model's performance. This project demonstrates the effectiveness of deep learning in recognizing emotions and provides a robust framework for further improvements and applications.

Dataset :-
I've used the FER-2013 dataset for training and evaluating our models. The dataset contains grayscale images of faces with seven different emotion labels: anger, disgust, fear, happiness, sadness, surprise, and neutral. Each image is resized to 48x48 pixels.

Preprocessing :-
- Normalization: Pixel values were scaled to the range [0, 1].
- Resizing: All images were resized to 48x48 pixels.
- Data augmentation: Techniques like rotation, zoom, horizontal flipping, and shift were applied to increase the diversity of the training set.

Model Architecture :- 
I've utilized the VGG16 and ResNet50 architectures for transfer learning. The top layers of these models were replaced with custom fully connected layers to adapt to the emotion classification task. 
- VGG16: The final dense layer was modified to output seven classes corresponding to the emotions.
- ResNet50: Similarly, the output layer was adjusted to match the number of emotion classes.

Data augmentation :- 
Data augmentation techniques were used to increase the training set diversity and prevent overfitting. The following augmentations were applied:
- Rotation (up to 30 degrees)
- Zoom (up to 20%)
- Horizontal flip
- Width and height shift (up to 20%)

Transfer Learning :-
Transfer learning was employed to leverage the feature extraction capabilities of pre-trained VGG16 and ResNet50 models. The pre-trained weights on the ImageNet dataset provided a strong starting point, enabling faster convergence and better performance on our emotion detection task.

Evaluation :-
Model performance was evaluated using accuracy, precision, recall, and F1-score. Confusion matrices were also generated to visualize the performance across different emotion classes.


