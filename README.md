# Natural-Language-Processing: 

Complete NLP understanding from end to end right from scratch till the advanced level

NLP: (Used with ML + DL) - NLTLK by Stanford, Spacy, Keras, Tensorflow, Pytorch

Text Processing Level 1: 	Tokenization, Lemmatization, Stop words Removal, POS. Finally 
Corpus. Machine cannot understand text. Hence next level.	
Stemming: History, Historical-Histori(Fast)
Lemmatization: History, Historical-History(Slow)
Packages:nltk,sklearn

Text Processing Level 2: 	Words to Vectors: BOW(Binary Bow, Normal Bow), TFIDF(), Unigrams, Bigrams, N grams. Importance & semantics is same for good &  boy in a sentence using BOW (I am a good boy). So TF( No: of rep of words in sentence/Total words in sentence). IDF (log(No of Sentences/No of sentences containing words))   Packages:nltk,sklearn(CountVectorizer,TfidfVectorizer)	 
Usage: Spam Ham Classifier(SMS Messages, Email Messages)

Text Processing Advanced: 	Word2Vec, AvgWord2Vec	"gensim: model.vv.most_similar('Sasi')
textblob : A Simple Api to do all above steps

Solving ML Usecases & ANN:
Sentiment Classifier, Document Classifier, Forecasting

RNN works very well with Sequence data. As above sequence of info is discarded.		
Usage: Chatbots, Q&A applications,Google Image Search, Google Translate, Speech Recognition

LSTM RNN:	Long Short Term Memory. Memory Cell, Forget Gate, Input Layer, Output Layer	
Packages: Tensorflow, Keras	

Word Embeddings	Word2Vec, Glove: Feature wise vectorization		

Bidirectional LSTM RNN:	If we have long sentences and the context of first word has dependency on last word.	If first word has imp at last word ,then only bidrectional. Else Slow, Not work well with speech recognition	

Sequence to Sequence Neural Networks: Encoders, Decoders	When a few features/ words is sent to LSTM, a context vector is created and then passed to LSTM of Decoder	Disadvantage is as the sentence length increases, the accuracy decreases.That is Bleu Score becomes low Hence attention models

Attention Models(Specified Time Frame), Transformers(Self Attention,feed fwd NN,Encoders, Decoders)	Bidirectional LSTM RNN as encoder , ANN with window time frame and decoder is an attention model. Window Size is considered for a specified time frame. Alpha values are initialised to be qqual to sum of all the values of Tx(TimeFrame) =1 (Softmax function is used) in a feed forward neural network.	Bleu score increased.
Usage: google translator.
Hyper Parameters: Time Stamp, No of encoders, no of decoders, vector dimension of features, dividing by 8 for queries score, single head attention /multi head.
