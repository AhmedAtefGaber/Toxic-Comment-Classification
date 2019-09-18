building a multi-headed model that’s capable of detecting different types of toxicity,The types of toxicity are:
- toxic
- severe_toxic
- obscene
- threat
- insult
- identity_hate 
Using dataset of a large number of Wikipedia comments have been labeled by human.
the input to the NN is the sentences after Tokenization and padding then pass it to an Embedding layer,
where it projects the words to a defined vector space depending on the distance of the surrounding words in a sentence. 
then pass the output of the Embeddingn to a Bidirectional LSTM then to two Dense Layers and using Dropout to reduce overfitting.
the Achieved Accuracy 98%.
