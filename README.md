# Project2
FinTech problem that machine learning can help solve : A comparitive analysis of various Crypto currencies BTC, ETC, ADA, USDT, XRP, LTC, TRX, TUSD, DGB, BSV using technical indicators including : Exponential Moving Averages in feature 1, Exponential Moving Average of Daily Return Volatility in feature 2, Bollinger Bands in feature 3 . A machine learning model based on the three signals : 'crossover_signal', 'vol_trend_signal', 'bollinger_signal' and setting the dependent variable values based on the logic where if daily return is greater than 0, then 1, else, 0. One year data is used to build the model. Then two sets of data are  Constructed the X_train and y_train. 

Then SKLearn linear regression using just the training set (X_train, Y_train) is used to fit the data. A confusion matrix, accuracy score is built. The predictions are calculated based on the model built for all the cryptos used in the sample. Graphs are plotted with the predicted values. The predicted values are replaced with -1 where 0 to depict the short situation which is the reverse of long positions. The cumulative return is then plotted.

Requirements of the project are below:
Apply ML in the context of technologies learned.
You must use: Scikit-Learn and/or another machine learning library.
You must use at least two of the below:
* Scikit-Learn
* Tensorflow
* Keras
* Google Colab
* Amazon SageMaker
* Amazon Lex

## Project Proposal

Write this as a brief summary of your interests and intent, including:

* The kind of data you'd like to work with and the field you're interested in (e.g., trading, quantitative analysis).

* Possible source for such data.

* Candidate machine learning or statistical models that you may want to explore.

> Our project is to predict credit card fraud. We'll fit a random forest algorithm to lending club data to create a predictive model. We will also fit a deep neural network model to the data and compare the performance of both models to determine which has sufficient predictive power.

## Finding Data

Once your group has written an outline, it's time to start hunting for data. You are free to use data from any source, but we recommend the following curated sources of high-quality data:

* [data.world](https://alpaca.markets/)

* [data.world](https://data.world/)

* [Kaggle](https://www.kaggle.com/)

* [Data.gov](https://www.data.gov)

* [Public APIs](https://github.com/abhishekbanthia/Public-APIs)

* [Awesome-APIs List](https://github.com/Kikobeats/awesome-api)

* [Medium APIs List](https://medium.com/@benjamin_libor/a-curated-collection-of-over-150-apis-to-build-great-products-fdcfa0f361bc)

Chances are you'll have to update your Project Outline as you explore the available data. This is fine—adjustments like this are part of the process! Just make sure everyone in the group is up to speed on the goals of the project as you make changes.

Make sure that your data is not too large for local analysis. Big-data datasets are difficult to manage locally, so consider a subset of that data or a different dataset altogether.

## Data Preparation & Model Training

Machine learning typically requires extensive data preparation before the model can be trained. Use Jupyter, Google Colab, or AWS SageMaker to prepare a training and testing dataset and to train the machine-learning model.

Use the training data to fit the model.

## Model Evaluation

Use the testing data to evaluate the model. Create any necessary tables, charts, plots, or statistical analysis to report the model performance.

## Predictions and Conclusions

Summarize your conclusions and predictions. This should include a numerical summary (what data your model yielded), as well as visualizations of that summary (plots of the final model evaluation and predictions).

Optionally, deploy the model as an interactive dashboard or interface (Lex or SageMaker).

Finally, be sure that your projects meet the [technical requirements](TechnicalRequirements.md).

## Presentation

After you've tweaked your model to your satisfaction, you'll put together a presentation to show off your work, explain your process, and discuss your conclusions.

This presentation will be delivered as a slideshow, and it should give your classmates and instructional staff an overview of your work. PowerPoint, Keynote, and Google Slides are all acceptable for building slides.

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

