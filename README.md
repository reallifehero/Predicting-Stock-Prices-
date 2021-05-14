# Predicting-Stock-Prices-
Overview

Trading in the stock market is one of the most fascinating endeavors I have ever undertaken. The pursuit of making money just by thinking is truly a mind-blowing journey. Stock market is no longer a venture undertaken by people in the wall street market floors wearing suits and ties. Anyone with access to a phone or a computer can trade in the markets now a days. This computerized trading brought more people to the markets and led to an abundance in algorithmic trading. In fact, "70% of all trades happening in the US are being handled by computerized systems."
What traders/investors want in the market is an edge (the higher probably of one thing happening over another). They do so using their own past experiences, reading current market conditions, and doing technical analysis of charts and price patterns. Since machines can process a lot more data and at a faster pace, they can definitely assist traders/investors to make better trading/investing decisions.
In this project, I will try to use an artificial recurrent neural network called Long Short Term Memory (LSTM) to predict the closing stock price of a company. My project will be done in Jupyter Notebook using Python as the programming language.
 
Dataset

The data was directly retrieved from yahoo finance's Api so I didn't have to download the data in my system which saves me some space in my local drive. To get the data, I needed to install pandas_datareader. Once I had the libraries and packages, I was able to connect and retrieve the raw data from the Yahoo. 

Methodology
Phase I 
Found and explored two sources of data: Quandl library and Yahoo Finance. Decided to stick to the Yahoo Finance dataset. 
Imported the libraries in Jupyter Notebook.
Retrieved the data and did some exploratory analysis. 
 
Phase II
Created a 30 and a 90 day moving average trend lines to find "sweet" to find sweet spots to buy and sell a stock
Prepare data for applying machine learning algorithm
Scale the the data/Create training and test data sets/reshape the data into 3-dimensions etc. 
Phase III  
 Build the LSTM model 
Compile the model 
Train the model 
Predict & get mean squared error to determine accuracy 

 
Literary Review /Exploratory Analysis/Applying Machine Algorithms

Personally, I have been an active trader in the market for the past 2 years and have read about 10 books on the stock market which equips me with some knowledge in the subject matter. As for the project, I have read quite a bit of literature in the topic of stock price prediction. I have also watched several videos on YouTube that present similar projects on the topic. The references section has the link to those articles and videos.
I’m doing some exploratory analysis using the pandas library and visualizing them using matplotlib. The machine learning algorithms as mentioned previously is Long Short Term Memory. Long short-term memory (LSTM) is an artificial recurrent neural network (RNN) architecture used in the field of deep learning. LSTM networks are well-suited to classifying, processing and making predictions based on time series data. LSTM models have really fascinating applications such as: speech recognition, robot control, grammar learning, and time series prediction. 

Results
There were two methods that I used in my code to predict stock prices. The first one was using long & term moving averages. There is this principle in trading that when the short term moving average crosses the long term moving average, it's a good time to buy. And when the long term crosses the short term, it's a good time to sell. This is depicted graphically in the chart. 
![image](https://user-images.githubusercontent.com/80177805/118150394-7f9d6600-b3e0-11eb-96bd-ffc4561de834.png)

The second method that I used is the machine learning algorithm LSTM. LSTM gave me the exact numbers with a margin of error obviously. The chart shows the actual and predicted prices. Besides the chart, I also used the algorithm to derive exact values as shown in the code. The margin of error that I used is called root mean squared error. In RMSE, a value of 0 is perfect score. My RMSE score is 10.31. 
![image](https://user-images.githubusercontent.com/80177805/118150487-9b087100-b3e0-11eb-8fd5-d5144831dbac.png)

Challenges 
There are couple of challenges I faced doing the project. Initially, I was confused about source of the data whether it's going to from quandl library or from yahoo. After doing some exploratory analysis, I had a better for yahoo data so I decided to stick to yahoo. 
This was my first type creating a github repository and making a youtube video. Even though they were comparatively easy that what I had in mind, I had to go through quite a few youtube videos and articles to successfully accomplish those tasks. I had downloaded gitbash but had trouble pushing the data online initially. I also had to learn to edit videos which I had never done before. 
Building and compiling the model was also a bit challenging. LSTM has multiple layers to it. You had to change the data from 2-dimension to 3-dimension. I had to some research on it and do some trial and error before I got it right. 



YouTube Presentations
https://www.youtube.com/watch?v=tefzXz-2X5Y -Phase I video 

https://www.youtube.com/watch?v=KYGx5jhjRbw -Phase II video 

https://www.youtube.com/watch?v=hRhmfNjcIwc -Phase III video 

 
References:
https://www.investopedia.com/articles/active-trading/101014/basics-algorithmic-trading-concepts-and-examples.asp
https://www.youtube.com/watch?v=SEQbb8w7VTw
https://www.youtube.com/watch?v=ftMq5ps503w
https://towardsdatascience.com/getting-rich-quick-with-machine-learning-and-stock-market-predictions-696802da94fe
https://www.analyticsvidhya.com/blog/2020/10/reinforcement-learning-stock-price-prediction/
 
