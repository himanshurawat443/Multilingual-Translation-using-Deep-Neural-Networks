# Multilingual-Translation-using-Deep-Neural-Networks
The objective of this project is to build a Text Language Translator where the input is a sequence of words and the output is translation of the given sequence in desired language. For this project we have taken Hindi, Gujarati & Marathi datasets from various sources which consists of 125,000 sentence pairs each.

Machine translation is the process of mechanically transforming source content provided in a particular language to textual form in desired language. Provided an arrangement of text in a particular source language we know that there can be multiple translation of that content in the desired language depending on the context and grammar. This is due to the natural uncertainty & adaptability of human level language makes the process of mechanized machine translation demanding & strenuous. 

Neural Machine Translation (NMT) utilizes neural networks to fabricate and train a sizable network that scans a sentence and generates a correct translation. The potency of NMT leans on it’s ability to remember relationships between input & output sentences , then plotting input to connected output text.

We did preprocessing on the dataset by converting everything to lowercase, removing quotes, numbers, text inside parenthesis, punctuations, special characters & extra spaces from text sequence for better training of the model.

During implementation of LSTM architecture a 3 Layer Stacked LSTM Encoder-Decoder model with Global Attention Mechanism was used. This model was able to reduce the loss and get an accuracy of **39.29%** on training set, generated predictions on test set which were poor and mostly inaccurate so we moved towards Transformer architecture. For implementation of Transformer we used a stack of 4 encoders & decoders each with attention mechanism & parallelization of data we were able to reduce loss & achieve accuracy of **79.52%** on training set, also generated highly accurate and mostly correct predictions on test set.

