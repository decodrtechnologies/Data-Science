# Amazon Musical Instruments Reviews Multiclass Classification


In this project, You have to implemente Long short-term memory (LSTM)  an artificial recurrent neural network (RNN) using __Keras__.

## Dataset

The data set can be downloaded by following link [Data](https://www.kaggle.com/eswarchandt/amazon-music-reviews)
he data set contains 10,261 instrument reviews from Amazon Database with rating labeled from 1 to 5.

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
[4, 80, 7, 6, 237, 165, 2, 39, 13, 12, 140, 143, 4, 1462, 2, 1749, 1426, 389, 328, 9, 17, 655, 60, 9, 12, 722, 97, 140]
I used it to hold down the strings on my bass while I adjusted the truss rod. Worked perfectly for that purpose. Works for my four string bass
```

## Building the model

We have used LSTM algorithm which will be explained in notebook.
The model has 9 layers (6 hidden layer) and 3 output layer .
I used `sigmoid` for the activation on the hidden layer, and `sigmoid` on the output layer.
Details are in the `notebook`.
Here's the summary of my model.

```
Model: "sequential_2"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
embedding_2 (Embedding)      (None, 120, 16)           160000    
_________________________________________________________________
bidirectional_2 (Bidirection (None, 64)                12544     
_________________________________________________________________
dense_4 (Dense)              (None, 6)                 390       
_________________________________________________________________
dense_5 (Dense)              (None, 3)                 21        
=================================================================
Total params: 172,955
Trainable params: 172,955
Non-trainable params: 0
_________________________________________________________________
```


## License
For more dataset information regarding license, please go through the following link,
https://creativecommons.org/publicdomain/zero/1.0/

