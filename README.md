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
```
