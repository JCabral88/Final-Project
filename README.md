# AI Contextual Chatbot - Cinebot

# CINEBOT🤖

This is my final project for the Ironhack Data Analysis Bootcamp that took place in the Summer of 2022.

The project consists on developing an AI Contextual Chatbot called Cinebot. His purpose is to provide you with information about a particular movie of interest, in a chat like experience.

So far Cinebot is programmed to provide informations about A.I. - Artificial Intelligence by Steven Spielberg, nevertheless the JSON file, which contains the data, can always be copied with new information about any other movie, giving this project room for improvment.

![Alt text](C:/Users/JoãoCabral/JC88Main/final_project/Final-Project/images/AImovie.jpg)

# Dataset📄

The dataset used in this project was built by myself on Visual Studio and saved in a JSON file. It will work as a python dictionary.
The data is structured in the following way:

- tag - Sets the classification and structure for bot response
- pattern - Bot identifies user input pattern
- response - Responses for the bot to reply (hardcoded). Result is a random output of the available responses.

![Alt text](C:/Users/JoãoCabral/JC88Main/final_project/Final-Project/images/Untitled.jpeg)

# Application Development🖥️

In order for Cinebot to understand human language, the dataset had to suffer several transformations before we start interacting with him.

The data went through several NLP stages for a model to be created and trained. Only this way the bot can understand and categorize the asked question.

This step of the project is where AI is implemented.

### NLP stage 1:

Natural Language Tool Kit - NLTK is a leading platform for building Python programs to work with human language data.

Tokenization with nltk ‘punkt’ - Divides a text into a list of sentences by using an unsupervised algorithm to build a model for abbreviation words, collocations, and words that start sentences.

Stemming with nltk  ‘LancasterStemmer()’ - Lancaster Stemmer is the most aggressive stemming algorithm, comparing with Porter and Snowball which were my alternatives.

Stemming generates the root from the word.

After above steps data can be gathered in a bag of words where the output is an array [0,1,1,0,0,…]

From here we are ready to go to the second stage of NLP.

### NLP stage 2:

With our structured bag of words we can now start to build our model to be trained and implemented. This way we enhance bot accuracy of replying the correct answer to the questions.

TFlearn is a modular deep learning library built on top of Tensorflow. It was designed to provide a higher-level API to TensorFlow in order to facilitate and speed-up experimentations, with TFlearn I have built a two layer Neural Network structure where the output is a model ready to be trained.

The model is than saved and ready to be applied.

![Alt text](C:/Users/JoãoCabral/JC88Main/final_project/Final-Project/images/chatbotbot.jpg)

# Adding Context🧐

In order to make life easier for the bot to reply I have created a context to user inputs.

This context, filters ‘tag’ content in the dataset and searches for best corresponse, this way the bot continues to provide a contextual approach to the conversation.

The user input is also victim of NLP for cleaning and structuring the text for bot analysis.
Those processes are tokenization and stemming.

# Conclusion🎓

Building this chatbot with NLP techniques help me do it in an easier way rather than using pre defined libraries of python. Applying a Neural Network with TFlearn structure definitely enhances the output result of the chatbot due to the several node layers accuracy in predicting the output.
There are still sereval ways that we can improve this chat bot, the first one is to add more different content to the dataset in order to have more information from more movies, the second one is to fit another model type, maybe from Keras, and check bot behaviour.

Overall Cinebot can be an easy and fast tool for you to have movie information at hand, this way you can beat your friends in an argument regarding an Oscar winner for example 😏

![Alt text](C:/Users/JoãoCabral/JC88Main/final_project/Final-Project/images/MovieNetflixGIF.gif)

# Sources🧭

- [investopedia.com/terms/c/chatbot.asp](http://www.investopedia.com/terms/c/chatbot.asp)
- [investopedia.com/terms/n/neuralnetwork.asp](https://www.investopedia.com/terms/n/neuralnetwork.asp)
- [youtube.com/watch?v=019a30EnNGk&ab_channel=TheAIUniversity](http://youtube.com/watch?v=019a30EnNGk&ab_channel=TheAIUniversity)
- [nltk.org](https://www.nltk.org/)
- [tensorflow.org](https://www.tensorflow.org/)
- [tflearn.org/models/dnn/](http://tflearn.org/models/dnn/)
- [edureka.co/blog/how-to-make-a-chatbot-in-python/](https://www.edureka.co/blog/how-to-make-a-chatbot-in-python/)
- [chatbotslife.com](https://chatbotslife.com/)

![Alt text](C:/Users/JoãoCabral/JC88Main/final_project/Final-Project/images/Sources.jpg)