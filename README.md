# HandWriting-Recognition-with-tensorflow
this is an handwriting recognition projects for digits and english letters


this is the number of x-train and y-tarin 
# the data, split between train and test sets
(x_train, y_train), (x_test, y_test) = mnist.load_data()
print(x_train.shape, y_train.shape)


then reshaped and categorized 
x_train shape: (60000, 28, 28, 1)
60000 train samples
10000 test samples
y_train shape: (60000, 10)
60000 train samples
10000 test samples


then conv2D and Maxpooling (we can also use average pooling but maxpooling retain the best case)
then compile and fit the model  and train the model 
Epoch 1/10
469/469 [==============================] - 135s 288ms/step - loss: 2.2670 - accuracy: 0.2006 - val_loss: 2.2223 - val_accuracy: 0.5048

Epoch 2/10
469/469 [==============================] - 135s 288ms/step - loss: 2.1925 - accuracy: 0.3527 - val_loss: 2.1288 - val_accuracy: 0.6240

Epoch 3/10
469/469 [==============================] - 136s 289ms/step - loss: 2.0918 - accuracy: 0.4653 - val_loss: 1.9955 - val_accuracy: 0.6726

Epoch 4/10
469/469 [==============================] - 137s 293ms/step - loss: 1.9473 - accuracy: 0.5445 - val_loss: 1.8069 - val_accuracy: 0.7098

Epoch 5/10
469/469 [==============================] - 136s 289ms/step - loss: 1.7517 - accuracy: 0.5957 - val_loss: 1.5639 - val_accuracy: 0.7416

Epoch 6/10
469/469 [==============================] - 135s 288ms/step - loss: 1.5226 - accuracy: 0.6374 - val_loss: 1.3010 - val_accuracy: 0.7756

Epoch 7/10
469/469 [==============================] - 136s 291ms/step - loss: 1.3018 - accuracy: 0.6695 - val_loss: 1.0705 - val_accuracy: 0.8002

Epoch 8/10
469/469 [==============================] - 136s 290ms/step - loss: 1.1258 - accuracy: 0.6957 - val_loss: 0.8959 - val_accuracy: 0.8177

Epoch 9/10
469/469 [==============================] - 136s 289ms/step - loss: 0.9931 - accuracy: 0.7196 - val_loss: 0.7725 - val_accuracy: 0.8292

Epoch 10/10
469/469 [==============================] - 135s 288ms/step - loss: 0.9009 - accuracy: 0.7364 - val_loss: 0.6845 - val_accuracy: 0.8406

The model has successfully trained

and after avalutae the model this is the result

Test loss: 0.684525191783905
Test accuracy: 0.8406000137329102
