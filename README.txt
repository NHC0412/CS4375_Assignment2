Sentiment Analysis Project


Table of Contents
Project Overview
Requirements
Installation Steps
Data Preparation
Running the Models
Plotting Results
Conclusion


Project Overview
This project implements a sentiment analysis task using a Feedforward Neural Network (FFNN) and a Recurrent Neural Network (RNN) to classify Yelp reviews into five sentiment classes. The project includes data preprocessing, model training, evaluation, and result visualization.


Requirements
To run this project, you need the following:
- Python 3.x
- Miniconda
- PyTorch
- NumPy
- Matplotlib
- JSON (for data handling)

Installation Steps

1. Install Miniconda:
Download and install Miniconda from the official website.

2. Create a Conda Environment: Open your command prompt and create a new environment:
conda create --name sentiment_analysis python=3.8

3. Activate the Environment: Activate your newly created environment:
conda activate sentiment_analysis

4. Install Required Packages: Install the necessary libraries using pip:
pip install torch numpy matplotlib


Data Preparation
Dataset: Place your JSON files (training.json, validation.json, test.json) in the same directory as your code files (ffnn.py and rnn.py).
Vectorization: The data will be vectorized in the scripts to convert text into numerical format suitable for model training.


Running the Models
1. Train the FFNN: To start training the Feedforward Neural Network, run the following command:
python ffnn.py --hidden_dim 50 --epochs 20 --train_data training.json --val_data validation.json --test_data test.json --do_train
python ffnn.py --hidden_dim 100 --epochs 20 --train_data training.json --val_data validation.json --test_data test.json --do_train

2. Train the RNN: To train the Recurrent Neural Network, run:
python rnn.py --hidden_dim 50 --epochs 20 --train_data training.json --val_data validation.json --test_data test.json --do_train
python rnn.py --hidden_dim 100 --epochs 20 --train_data training.json --val_data validation.json --test_data test.json --do_train


