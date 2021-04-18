It is an extension of the [[word2vec]] that tries to solve encoding of unknown words.

Unlike the [[word2vec]] it does not feed the whole words to the model, but the [[n-gram]]s. The n-grams of unknown words have a high probability to be similar to the n-grams of known words with a similar meaning.