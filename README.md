# Car Price Estimation

This GitHub repository contains a Python-based car price estimation project that utilizes web scraping from a car-selling website, data processing, and machine learning techniques to predict the prices of used cars. The project aims to provide a practical tool for estimating car prices based on various attributes.

## Table of Contents

- [Introduction](#introduction)
- [Project Overview](#project-overview)
- [Technologies Used](#technologies-used)
- [How to Use](#how-to-use)
- [Conclusion](#conclusion)

## Introduction

Estimating the price of used cars is a valuable task for both buyers and sellers. This project utilizes web scraping techniques, machine learning, and data preprocessing to achieve this goal. The key steps involve extracting car data from a website, cleaning and processing the data, training a machine-learning model, and creating a prediction function.

## Project Overview

The project involves the following major steps:

1. **Data Scraping:**
   - The code utilizes Beautiful Soup and requests libraries to extract car data from the TrueCar website.
   - Extracting information like VIN, car model, year, mileage, accidents, owners, and price.

2. **Data Preprocessing:**
   - Cleaning and processing the scraped data to handle missing values and format the features appropriately.
   - Extracting and utilizing attributes like the number of accidents and owners from the provided text using regular expressions.

3. **Database Integration:**
   - Storing the extracted car data into a MySQL database for further analysis.

4. **Creating CSV from SQL:**
   - Transforming the SQL table into a CSV file for easier handling and analysis.

5. **Data Analysis:**
   - Loading the CSV data into a Pandas DataFrame and analyzing the data.
   - Filtering the dataset based on the number of repetitions to ensure a balanced dataset.

6. **Data Splitting and Processing:**
   - Splitting the dataset into training and testing sets.
   - Scaling numerical attributes and encoding categorical ones for machine learning.

7. **Machine Learning Model:**
   - Training a linear regression model on the training dataset. The model learns to predict car prices based on the provided attributes.
   - Evaluating the model on the testing dataset using Mean Squared Error and Mean Absolute Error.

8. **Prediction Function:**
   - Creating a function to predict the price of new cars based on given attributes. Users can input a car's model, manufacture year, and mileage to get a price estimate.

## Technologies Used

The project employs several technologies and best practices, including:

- **Python**: The core language used for development.
- **Web Scraping**: The project leverages web scraping to gather car data from the TrueCar website.
- **MySQL**: A database is used to store and manage the collected car data.
- **Pandas and NumPy**: Data manipulation and analysis libraries are used to process and filter the scraped data.
- **Scikit-Learn**: A machine learning library is used to build and evaluate a linear regression model for price prediction.
- **Regular Expressions**: Regular expressions are used to extract relevant information from the web pages.
- **Data Scaling and Encoding**: Standard scaling and one-hot encoding are applied to prepare the data for machine learning.
- **CSV Data Export**: Car data is exported to a CSV file for further analysis and model training.

## How to Use

1. Input the name of the car model.
2. The script will scrape car data from the specified website.
3. It will preprocess the data, handle missing values, and store the data in a MySQL database.
4. The script will create a CSV file from the SQL table and analyze the data.
5. Data will be split, processed, and used to train a machine learning model (linear regression).
6. The provided prediction function can be used to predict the price of a new car.

## Conclusion

This car price estimation project combines web scraping, data processing, and machine learning to predict used car prices. By following the steps outlined in this README, you can gain insights into how to estimate car prices and leverage the provided code for your own applications. Feel free to explore and extend the project as needed.
