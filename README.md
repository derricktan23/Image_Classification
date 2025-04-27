TensorFlow Flower Classification
# Flower Classification with TensorFlow

This project uses TensorFlow and Keras to classify images of flowers (daisy, dandelion, rose, sunflower, tulip).  
It covers data download, preprocessing, model building, training, evaluation, and prediction.

**To download the dataset:**
```
import tensorflow as tf
dataset_url = "https://storage.googleapis.com/download.tensorflow.org/example_images/flower_photos.tgz"
data_dir = tf.keras.utils.get_file('flower_photos', origin=dataset_url, untar=True)
```

Train your model and predict flower types from images with just a few lines of code!


# Flower Classification with TensorFlow

This project demonstrates image classification of flowers using TensorFlow and Keras.

## Steps

1. **Import Libraries**  
   Import TensorFlow, Keras, NumPy, Matplotlib, and PIL for data handling and modeling.

2. **Download & Explore Dataset**  
   Download the [flowers dataset](https://storage.googleapis.com/download.tensorflow.org/example_images/flower_photos.tgz), which contains five classes: daisy, dandelion, roses, sunflowers, tulips. Visualize and count images.

3. **Prepare Data**  
   Use `image_dataset_from_directory` to load images, split into training (80%) and validation (20%) sets, and display class names.

4. **Optimize Data Pipeline**  
   Apply `.cache()` and `.prefetch()` for efficient data loading. Standardize images to [0, 1] range.

5. **Build Model**  
   Create a Sequential CNN with convolution, pooling, flatten, and dense layers.

6. **Compile Model**  
   Use Adam optimizer and sparse categorical cross-entropy loss.

7. **Train Model**  
   Train for several epochs, tracking accuracy and loss.

8. **Visualize Results**  
   Plot training and validation accuracy/loss.

9. **Improve Model**  
   Add data augmentation and dropout layers for better generalization and retrain.

10. **Test Model**  
    Predict the class of a new flower image and display the result.

---
