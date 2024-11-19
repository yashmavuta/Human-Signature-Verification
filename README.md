# Human-Signature-Verification
#### Neural Networks: CNNs (Convolutional Neural Networks) are commonly used for signature verification due to their ability to effectively learn hierarchical patterns and features from images.
#### The script begins by loading a dataset from a pickle file named "signatures 2.pkl" that contains images and their corresponding labels.
#### The data is then split into training and testing sets using a 80-20 split ratio. labels -= 1: This code snippet subtracts 1 from all elements in the labels array. This operation suggests that the labels might have started from 1 and this operation aligns them to start from 0, which is common in machine learning when indexing starts from 0.
#### Model Architecture: Sequential Model Creation: A linear stack of layers is represented by the instantiation of a sequential model.
#### Convolutional Layers: ReLU activation functions are used to create two convolutional layers (Conv2D), respectively. These layers use the incoming images to learn hierarchical representations.
#### MaxPooling Layers: A max-pooling layer (MaxPooling2D) decreases the spatial dimensions of the representations after each convolutional layer, preserving significant information while lowering computational cost.
#### The flatten layer is responsible for transforming the convolutional layer's output into a vector that can be incorporated into the dense layers.
#### Dense Layers: ReLU activation functions are present in two dense (completely linked) layers. For multiclass classification, the final dense layer has a softmax activation function with nine units (assuming there are nine classes).
