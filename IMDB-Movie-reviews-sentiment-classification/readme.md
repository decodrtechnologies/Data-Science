# IMDB-Movie-reviews-sentiment-classification


In this project, I implemented Long short-term memory (LSTM) is an artificial recurrent neural network (RNN) using __Keras__.

## Dataset

The data set contains 50,000 movie reviews from Internet Movie Database (IMDB) labeled whether they are positive or negative.
Each review is preprocessed to be encoded as a sequence of word indexes.
For instance, let there be a sentence "To be or not to be".
The mapping of the words are as follows:

- to: 2
- be: 6
- or: 19
- not: 10

The above sentence "To be or not to be" is encoded as `[2, 6, 19, 10, 2, 6]`.

## Data Processing

The data is processed by converting in integer sequence using tokenizer and word_index function and then padded and truncated for eg lets say that if the review is of 10 words and another is of 12 words now to make sure that the length will remain same we have use padding and truncating and fixed the length of the training and test sequences which will be explained in notebook.

Example of a training example how it is converted in integer from text.

```
[59, 12, 14, 35, 439, 400, 18, 174, 29, 1, 9, 33, 1378, 3401, 42, 496, 1, 197, 25, 88, 156, 19, 12, 211, 340, 29, 70, 248, 213, 9, 486, 62, 70, 88, 116, 99, 24, 5740, 12, 3317, 657, 777, 12, 18, 7, 35, 406, 8228, 178, 2477, 426, 2, 92, 1253, 140, 72, 149, 55, 2, 1, 7525, 72, 229, 70, 2962, 16, 1, 2880, 1, 1, 1506, 4998, 3, 40, 3947, 119, 1608, 17, 3401, 14, 163, 19, 4, 1253, 927, 7986, 9, 4, 18, 13, 14, 4200, 5, 102, 148, 1237, 11, 240, 692, 13, 44, 25, 101, 39, 12, 7232, 1, 39, 1378, 1, 52, 409, 11, 99, 1214, 874, 145, 10]
b"This was an absolutely terrible movie. Don't be lured in by Christopher Walken or Michael Ironside. Both are great actors, but this must simply be their worst role in history. Even their great acting could not redeem this movie's ridiculous storyline. This movie is an early nineties US propaganda piece. The most pathetic scenes were those when the Columbian rebels were making their cases for revolutions. Maria Conchita Alonso appeared phony, and her pseudo-love affair with Walken was nothing but a pathetic emotional plug in a movie that was devoid of any real meaning. I am disappointed that there are movies like this, ruining actor's like Christopher Walken's good name. I could barely sit through it."
```

## Building the model

We have used LSTM algorith which will be explained in notebook.
The model has 7 layers (6 hidden layer) .
I used `relu` for the activation on the hidden layer, and `sigmoid` on the output layer.
Details are in the `notebook`.
Here's the summary of my model.

```
Model: "sequential"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
embedding (Embedding)        (None, 120, 16)           160000    
_________________________________________________________________
bidirectional (Bidirectional (None, 64)                12544     
_________________________________________________________________
dense (Dense)                (None, 6)                 390       
_________________________________________________________________
dense_1 (Dense)              (None, 1)                 7         
=================================================================
Total params: 172,941
Trainable params: 172,941
Non-trainable params: 0
_________________________________________________________________
```

## Training and validating the model

I trained the model  for only 5 epochs.
Here's result of the training for the five epochs. 

```
Epoch 1/5
782/782 [==============================] - 75s 95ms/step - loss: 0.1147 - accuracy: 0.9614 - val_loss: 0.4856 - val_accuracy: 0.8281
Epoch 2/5
782/782 [==============================] - 71s 91ms/step - loss: 0.0820 - accuracy: 0.9712 - val_loss: 0.6072 - val_accuracy: 0.8244
Epoch 3/5
782/782 [==============================] - 73s 93ms/step - loss: 0.0579 - accuracy: 0.9804 - val_loss: 0.6630 - val_accuracy: 0.8083
Epoch 4/5
782/782 [==============================] - 70s 90ms/step - loss: 0.0397 - accuracy: 0.9871 - val_loss: 0.7662 - val_accuracy: 0.8167
Epoch 5/5
782/782 [==============================] - 69s 88ms/step - loss: 0.0313 - accuracy: 0.9900 - val_loss: 0.8376 - val_accuracy: 0.8178
```



