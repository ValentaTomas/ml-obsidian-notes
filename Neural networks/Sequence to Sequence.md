Sequence to Sequence [[Deep learning]] models take a sequence of items (letters, words, features of images...) and outputs another sequence of items.

This is used for example in the neural machine translation.

The model is compose of an [[Encoder]] and [[Decoder]]. These are usually [[Recurrent Neural Network]]s that accept the previous word's context as a next word's hidden state input. 