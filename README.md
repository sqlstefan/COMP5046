# COMP5046 Assignment 1 [Individual Assessment]

<b>[XXX] = Lecture/Lab Reference</b><br/>
<b>(Justify your decision) = Please justify your decision/selection in the documentation</b>


<h1>Sentiment Analysis using Recurrent Neural Networks</h1>
<p><b>In this assignment1, we will focus on developing sentiment analysis model using Recurrent Neural Networks (RNN). </b><br/>
Sentiment analysis <b>[Lecture5]</b> is contextual mining of text which identifies and extracts subjective information in source material, and helps a business to understand the social sentiment of their brand, product or service while monitoring online conversations.<br/><br/>
<i>For your information, the detailed information for each implementation step was specified in the following sections. Note that lab exercises would be a good starting point for the assignment. The useful lab exercises are specified in each section.</i></p>

<br/>
<br/>

<h2>1. Data Preprocessing</h2>
<p>In this assignment, you are to use the <b>NLTK's Twitter_Sample</b> dataset. Twitter is well-known microblog service that allows public data to be collected via APIs. NLTK's twitter corpus currently contains a sample of Tweets retrieved from the Twitter Streaming API. If you want to know the more detailed info for the nltk.corpus, please check the <a href="https://www.nltk.org/howto/corpus.html">nltk website</a>.<br/>
The dataset contains twitter posts (tweets) along with their associated binary sentiment polarity labels. Both the training and testing sets are provided in the form of pickle files (testing_data.pkl, training_data.pkl) and can be downloaded from the Google Drive using the provided code in the <b><a href="https://colab.research.google.com/drive/1A6azpUOCUU923JF5B4v7t2pNSzLAQ20t?usp=sharing">Assignment 1 Template ipynb</a></b>.</p>
<p>
In this Data Preprocessing section, you are required to implement the following functions:</br>
<ul>
  <li><b>Preprocess data</b>: You are asked to pre-process the training set by integrating several text pre-processing techniques <b><i>[Lab5]</i></b> (e.g. tokenisation, removing numbers, converting to lowercase, removing stop words, stemming, etc.). You should justify the reason why you apply the specific preprocessing techniques <b>(Justify your decision)</b>
  </li>
 </ul>
</p>


<br/>
<br/>


<h2>2. Model Implementation</h2>
<p>In this section, you are to implement three components, including Word Embedding module, Lexicon Embedding module, and Bi-directional RNN Sequence model. For training, you are free to choose hyperparameters <b><i>[Lab5]</i></b> (e.g. size of vector for embeddings, learning rate, epochs, etc.)</p>

<h3>1)Word Embedding</h3>
First, you are asked to build the word embedding model (for representing word vectors, such as word2vec-CBOW, word2vec-Skip gram, fastText, and Glove) for the input embedding of your sequence model <b><i>[Lab2]</i></b>. Note that we used a one-hot vector as an input for the sequence model <i>in the Lab3 and Lab4</i>. In order to build the word embedding model, you are required to implement the following functions:
<ul>
  <li><b>Preprocess data for word embeddings</b>: You are to use and preprocess NLTK Twitter dataset (the one provided in the <i>Section 1</i>) for word embeddings  <b><i>[Lab2, Lab3]</i></b>. This can be different from the preprocessing technique that you used in Section 1. You can use both training and testing dataset in order to train the word embedding. <b>(Justify your decision)</b> </li>
  
  <li><b>Build training model for word embeddings</b>: You are to build the training model for word embeddings. You are required to articulate the hyperparameters <b><i>[Lab4]</i></b> you chose (size of vector for embeddings, learning rate, etc.). Note that any word embeddings model <b><i>[Lab2]</i></b> (e.g. word2vec-CBOW, word2vec-Skip gram, fasttext, glove) can be applied. <b>(Justify your decision)</b> </li>
  
  <li><b>Train model</b>: You are to train the model in PyTorch.</li>
</ul>
  

<h3>2)Word Embedding</h3>
First, you are asked to b



While the model is being trained, you are required to display the Training Loss and the Number of Epochs. 



<h2>3. Evaluation</h2>
<p>In this assignment, you are to use the [dataset description]</p>


<h2>4. Documentation</h2>
<p>In the section 1,2, and 3, you are required to describe and justify any decisions you made for the final implementation. You can find the tag ‘[Justify your decision]’ for the point that you should justify the purpose of applying the specific technique/model.<br/>
For example, for section 1 (preprocess data), you need to describe which pre-processing techniques (removing numbers, converting to lowercase, removing stop words, stemming, etc.) were conducted and justify your decision (the purpose of choosing a specific pre-processing techniques, and benefit of using that technique or the integration of techniques for your AI) in your ipynb file</p>
  


<h2>Submission Instruction</h2>
<p>The following are the submission files and description of each files</p><br/>
<ul>
  <li>ipynb file - (file name: your_unikey_COMP5046_Ass1.ipynb)</li>
  <li>model zip file</li>
  <li>l zip file</li>
</ul>

<p>Submit a ipynb file that contains all above sections(Section 1,2,3,4 and 5).<br/>
  The ipynb template can be found in the <a href="https://colab.research.google.com/drive/1A6azpUOCUU923JF5B4v7t2pNSzLAQ20t?usp=sharing">Assignment 1 template</a></p>
