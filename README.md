# Predicting Hotel Booking Cancellations

This project is a part of the ADS-505 course in the Applied Data Science Program at the University of San Diego.

**Project Status: Completed**

## Installation
1. Clone the repository:
   ```
   git clone https://github.com/sascott9655/ADS-505-Hotel_Bookings_Project.git
   ```
2. Install the required packages (Python 3.11+):
   ```
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```
3. Open `ADS_505_Final_Notebook.ipynb` and select **Restart Kernel and Run All**. The data loads directly from this repository, and a full run takes about 1–2 minutes.

## Project Intro/Objective
The goal of this project is to predict which hotel bookings are likely to be canceled and understand what drives those cancellations. We tuned our models for precision, so that when a booking is flagged, the hotel can trust it enough to act, such as overbooking the room, without risking guests showing up to no room.

## Contributors
- **Guillermo Alejandro Valencia:** logistic regression, shared data split and results framework, merging notebooks
- **Brandon [Last Name]:** Naive Bayes, group-based split for duplicate bookings
- **Samuel Scott:** neural network, model comparison, final test evaluation

## Methods Used
- Exploratory Data Analysis
- Data Visualization
- Predictive Modeling
- Machine Learning (Logistic Regression, Naive Bayes, Neural Networks)

## Technologies
- Python, Jupyter Notebook
- pandas, NumPy, Matplotlib, seaborn, scikit-learn

## Project Description
The dataset contains 119,390 bookings with 32 variables from a City Hotel and a Resort Hotel in Portugal (2015–2017). We explored which booking characteristics are linked to cancellations, then built logistic regression, Naive Bayes and neural network models for each hotel. Models were compared on a validation set at 90% precision, and the neural network performed best.

The main challenges were duplicate rows from group bookings (kept, with a group-based split so copies never landed in both training and test data), columns that leaked the outcome (removed), and Resort cancellations being much harder to predict confidently than City cancellations.

## Data Source
Antonio, N., de Almeida, A., & Nunes, L. (2019). Hotel booking demand datasets. *Data in Brief, 22*, 41–49. https://doi.org/10.1016/j.dib.2018.11.126
