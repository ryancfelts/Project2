# Project2
FinTech problem that machine learning can help solve : An analysis of various Crypto currencies BTC, ETC, ADA, USDT, XRP, LTC, TRX, TUSD, DGB, BSV using technical indicators including : Exponential Moving Averages in feature 1, Exponential Moving Average of Daily Return Volatility in feature 2, Bollinger Bands in feature 3 . A machine learning model Random Forest Trading based on the three signals : 'crossover_signal', 'vol_trend_signal', 'bollinger_signal' and setting the dependent variable values based on the logic where if daily return is greater than 0, then 1, else, 0. One year data is used to build the model. Then two sets of data are  Constructed the X_train and y_train. 

Then SKLearn linear regression using just the training set (X_train, Y_train) is used to fit the data. A confusion matrix, accuracy score is built. The predictions are calculated based on the model built for all the cryptos used in the sample. Graphs are plotted with the predicted values. The predicted values are replaced with -1 where 0 to depict the short situation which is the reverse of long positions. The cumulative return is then plotted.

Requirements of the project are below:
Apply ML in the context of technologies learned.
You must use: Scikit-Learn and/or another machine learning library (Used MinMaxScaler Model)
You must use at least two of the below:
* Scikit-Learn
* Tensorflow
* Keras
* Google Colab
* Amazon SageMaker
* Amazon Lex
 
 Apart from the Cryptos described above, we also chose the top 10 market cap stocks to use the "LSTM Stock Predictor" Using Closing Prices and build the model. The stocks are : tickers "AAPL","MSFT","AMZN","GOOG","FB","TSLA","BRK.A","V","JPM","JNJ". These are the top 10 US stocks on the NYSE by MarketCap found on  stock found http://www.iweblists.com/us/commerce/MarketCapitalization.html.

## Project Proposal

We are interested in building Machine Learning based models , combine with algorithmic / quantitative trading aspects and evolve an automated buy/sell signal generator or predcitive stock/crypto prices.
* We chose some of the top traded cryptos and 10 stocks by market capitablization for this project. Shrimpy apis , Alcapa trades apis have been the primary sources to load data for the cryptos and stocks respectively. We'll fit a random forest algorithm to cryptos data from shrimpy  to create a predictive model with iterative features.

## Finding Data

Our team based the data collection to 

* [data.world](https://www.shrimpy.io/dashboard)

## Data Preparation & Model Training

Machine learning typically requires extensive data preparation before the model can be trained. We used  Jupyter , Google Colab to prepare a training and testing dataset and to train the machine-learning models.  The training data was used to fit the model. The notebook references are : CryptoData.ipynb for fetching the data, CryptoCleaning.ipynb was used to make data suitable for analysis including dropping nulls and other such cleansing processes. CryptoAnalysis.ipynb was used to conduct the initial analysis and preparing the test , train data to be available to fit the model. ModelBUilding.ipynb hosts the model built.

We used Google Colab to prepare data in  Top10_MarketCap_Model.ipynb. LSTM(Long Short Term Memmory based predictor model was used to fit the data. An interesting article on LSTM : https://colah.github.io/posts/2015-08-Understanding-LSTMs/#:~:text=Long%20Short%20Term%20Memory%20networks,many%20people%20in%20following%20work.
 

## Model Evaluation

The testing data to evaluate the model. Created  necessary tables, charts, plots, or statistical analysis to report the model performance.

## Predictions and Conclusions

Summarize your conclusions and predictions. This should include a numerical summary (what data your model yielded), as well as visualizations of that summary (plots of the final model evaluation and predictions).

## Presentation

Guidelines:
As long as your slides meet the [presentation requirements](PresentationRequirements.md), you are free to structure the presentation however you wish, but students are often successful with the format laid out in the [presentation guidelines](PresentationGuidelines.md).

## Submission

In addition to submitting your project on Bootcamp Spot individually, please [fill out this form](https://forms.gle/CBk5tyy4sSsGN8k38) **once per group**.

## Contributing
Francene, Ryan and Murthy contributed to this project apart from invaluable guidance from Instructors: Steve and Kowsi. We also would like to thank all the other students in our class for all the interactions and creative ideas that made this possible.

## Licencing
No licencing requirements exists for this version of the project deliverables

# Technical Requirements

The technical requirements for Project 2 are as follows.

* [ ] Create a Jupyter Notebook, Google Colab Notebook, or Amazon SageMaker Notebook to prepare a training and testing dataset.

* [ ] Optionally, apply a dimensionality reduction technique to reduce the input features, or perform feature engineering to generate new features to train the model.

* [ ] Create one or more machine learning models.

* [ ] Fit the model(s) to the training data.

* [ ] Evaluate the trained model(s) using testing data. Include any calculations, metrics, or visualizations needed to evaluate the performance.

* [ ] Show the predictions using a sample of new data. Compare the predictions if more than one model is used.

* [ ] Save PNG images of your visualizations to distribute to the class and instructional team and for inclusion in your presentation and your repo's README.md file.

* [ ] Use one new machine learning library, machine learning model, or evaluation metric that hasn't been covered in class.

* [ ] Create a README.md in your repo with a write-up summarizing your project. Be sure to include any usage instructions to set up and use the model.

# Presentation Requirements

The presentation requirements for the project are as follows.

* [ ] Be at least 8 to 10 minutes long (check with the instructor for the official presentation time).

* [ ] Describe the core message or hypothesis for your project.

* [ ] Describe the predictive model chose and why this model was chosen.

* [ ] Describe the data preparation and model training process.

* [ ] Describe the techniques used to evaluate the model performance.

* [ ] Summarize your conclusions and predictions. This should include a numerical summary (what data your model yielded), as well as visualizations of that summary (plots of the final model evaluation and predictions).

* [ ] Discuss the implications of your findings. This is where you get to have an open-ended discussion about what your findings mean.

# Presentation Guidelines

You are free to structure your presentations to your liking, but students tend to have success with the following format.

* Title Slide

  * Include the name of the project and group members.

* Motivation & Summary Slide

  * Define the core message or hypothesis of your project.

* Model Summary

  * Elaborate on the predictive model used, describing why it was the best choice for the data.

* Data Cleanup & Model Training

  * Describe the exploration and cleanup process.
  * Discuss any problems that arose with preparing the data or training the model that you didn't anticipate.
  * Discuss the overall training process and highlight anything of interest with the training process: Cloud resources used, training time required, issues with training.

* Model Evaluation

  * Discuss the techniques you used to evaluate the model performance.

* Discussion

  * Discuss your findings. Was the model sufficient for the predictive task? If not, why not? What inferences or general conclusions can you draw from your model performance?

* Postmortem

  * Discuss any difficulties that arose, and how you dealt with them.
  * Discuss any additional questions or problems that came up but you didn't have time to answer: What would you research next if you had two more weeks?

* Questions

  * Open-floor Q&A with the audience.

