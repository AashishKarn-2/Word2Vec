Source and support: https://youtu.be/DDfLc5AHoJI
## Word Embedding

Word embedding is a technique used in natural language processing **to represent words as numerical vectors.** These vectors are created by analyzing large amounts of text data and identifying patterns in how words are used together. **Each word is then assigned a vector based on its relationship to other words in the text.** This allows computers **to understand the meaning and context of words,** which is useful for tasks like **language translation and sentiment analysis**. Word embedding has become an important tool in the field of natural language processing and has helped to advance the development of more advanced language technologies.

1. **Word2VEC**

**Word2vec** is a popular technique used in natural language processing to represent words as numerical vectors. It is a neural network-based method that learns word embeddings from large amounts of text data. Word2vec has become an important tool in the field of natural language processing and has helped to advance the development of more advanced language technologies.

Word2vec works by considering the context in which words appear in a text corpus. The neural network is trained to predict the probability of a word appearing in a given context, given the surrounding words. This allows the network to learn word embeddings that capture the relationships between words in the text.

Once the word embeddings have been learned, they can be used in a variety of natural language processing tasks. For example, word embeddings can be used to find words that are semantically similar to one another, or to identify words that frequently appear together in a given context. Word embeddings can also be used to improve the accuracy of machine learning models used in natural language processing, such as sentiment analysis or language translation.

Word2vec has become a popular tool in natural language processing due to its ability to capture complex relationships between words in a text corpus. It has been used in a variety of applications, from predicting the next word in a sentence to improving the accuracy of machine translation models. As the field of natural language processing continues to advance, it is likely that word2vec and other word embedding techniques will continue to play an important role in the development of more advanced language technologies.




![Untitled (2)](https://github.com/Aashish-compo/Word2Vec/assets/64850093/4b56be9a-7d82-4231-9d13-398c79f478f5)

Below we see that from google news dataset we have 300 number’s vector is used for the representation of one word and someone has extracted only 50 features and encoded it. It has make 300 features. We have extracted 50 features which is color coded.
INTERESTING: WE NEVER KNOW WHAT THAT FEATURE IS BUT THAT’S A FEATURE

The two ways of doing word2vec are:

1. Continuous Bag of Words (CBOW)
2. Skip-gram

**CBOW**

Steps for doing word2vec

1. Convert each word to the one hot encoded form
2. Create a Fake problem where 1st and 3rd word are input and second word is output
3. eg: I am a boy. **“I”** and **“a”** is input and **“am”** is output.
4. Finally we feed the encoded form of the **“I”** and **“a”** as input in neural net and gets the weight.
5. Now output layer consist of the all vocabulary. Now the weight connected between Hidden layer and Last layer is final vector representation of that word. In Below case [w1, w2, w3] is vector representation of the watch 
![Untitled (6)](https://github.com/Aashish-compo/Word2Vec/assets/64850093/25dbd618-7344-4131-a6e4-be0f8c4f4ea9)

**Skip-gram**

In skip-gram same thing is done but now we make middle word as input and side two words as output.
![Untitled (1)](https://github.com/Aashish-compo/Word2Vec/assets/64850093/73735dfe-a83f-408a-bdae-d35b872f6d90)
HERE → 1st layers weight is assigned as the vector of the individually input word.

NOTE: CBOW is generally used for small data and Skip-gram is used for larger dataset.





