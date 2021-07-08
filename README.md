# Deep Learning for Bitcoin Price Movement Prediction

## About

This is a project that was carried out for the "Computational Intelligence" class in the 8th semester of the School of Informatics at the Aristotle University of Thessaloniki.
The goal was to predict the direction in which the price of Bitcoin would move at a given day, whether that would be upwards or downwards, using Deep Learning techniques such as MLPs, LSTMs and CNNs.

In this repository, you will find:

- a Python notebook (.ipynb) with the code

- a detailed study report (.pdf) in Greek

- all of the dataset files used (.csv)

- an [Anaconda](https://www.anaconda.com/) environment file (.yml)

## Environment

### Local setup

In order to set up the environment locally, you can use the `environment.yml` file with Anaconda.

Additionally, you will have to install **pandas_ta** using pip:

```sh
$ pip install pandas_ta
```

If you want to use the **pytrends** module to load data from Google Trends, it will have to be installed through pip as well.
However, there is a CSV file (`_google.csv`) with all historical data up to May 2020 included in this repository's files, which can be used to save time, as retrieving this information is quite a slow process due to Google's rate limit.

### Google Colab

Instead of setting everything up locally, it is highly recommended that you use [Google Colab](https://research.google.com/colaboratory/) since it both offers a hosted runtime **with GPUs** that you can use for free, and also it has all of the required libraries pre-installed (except for pandas_ta and pytrends, which can be installed within the Python notebook by executing the corresponding cells).

This option should be preferred, especially if you are not experienced with managing Python libraries, or most importantly if you don't have a powerful GPU, since the DL models used take quite a while to be trained on a CPU-only machine.
