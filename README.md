# News-Article-Source-Prediction

When we go through a news article online, we are always concerned whether our news is coming from the right source.
Media stack has news articles from multiples sources/channels. Our goal is to train ML models that can predict the source of the news based on the content provided.

## Data

We have around 26k data points belonging to 8 sources, fetched from Media Stack site using API. 
- Below we can see number of articles beloning to different news sources and categories.
![image](https://user-images.githubusercontent.com/57527313/222935132-3d9b76ea-1fb9-407b-882e-bc78f3cbb6dc.png)

- Below we can the distrubution of articles based on number of words in each of them.
![image](https://user-images.githubusercontent.com/57527313/222935137-70054944-9771-412a-abdd-f4e5d88d0b56.png)


## Model Trained

To convert textual information to numerical vectors we tried both glove embedding, with all sizes, and keras inbuild embedding, out of which keras inbuild embedding performed well.

Split the data by 75/25 ratio to training and validation datasets

We tried below models
- Keras sequential with embedding size [100,200,300,400]
- RNN & Multilayer RNN
- LSTM & Bi-driectional LSTM
- 1d-CNN
- 1d-CNN with Bi-driectional LSTM

## Results

- We have tried multiple combinations of deep learning neural networks such as LSTM, biLSTM & CNN.
- We have also tried glove embedding, the code for it is present in this google colab notebook, ---https://colab.research.google.com/drive/1Sg5IdCBNjy1eYdwVDPLQ9xXfUnNdxkTC?usp=sharing
- As we can see from the graph the best performance is achieved by Keras Model with embedding size 100, i.e. NN_embd_100

![image](https://user-images.githubusercontent.com/57527313/222935191-47001c7a-1475-4964-851d-d7498737e342.png)
