# House Price Prediction

This project aims to predict house prices in Egypt using various features of the houses such as area, number of bedrooms, bathrooms, and type of house. The project employs data preprocessing techniques and applies linear regression models to make predictions.

## Project Structure

- `Egypt_Houses_Price.csv`: The dataset containing information about houses in Egypt.
- `project.py`: The main script for data preprocessing, model training, and evaluation.
- `README.md`: This file, providing an overview of the project.
- `AddVenvToJupyter.txt`: Add env to ur project using conda.

## Dataset

The dataset includes the following columns:
- `Area`: The area of the house.
- `Bedrooms`: Number of bedrooms.
- `Bathrooms`: Number of bathrooms.
- `Level`: The floor level of the house.
- `Type`: The type of the house (e.g., Apartment, Duplex, Stand Alone Villa, Chalet).
- `Price`: The price of the house.

## Preprocessing Steps

1. **Data Cleaning**: Replace specific values in the 'Level' column and filter out rows that do not match the specified house types.
2. **Encoding**: Convert the 'Type' column to dummy variables.
3. **Feature Engineering**: Add a 'Total Rooms' feature by summing the number of bedrooms and bathrooms.
4. **Splitting Data**: Split the dataset into training and testing sets.

## Model Training

- **Linear Regression**: A simple linear regression model is trained on the preprocessed data.
- **Polynomial Features**: Polynomial features of degree 2 are generated and used to train the model.

## Usage

1. Clone the repository:
    ```sh
    git clone https://github.com/f-agour/house-price-prediction.git
    ```
2. Navigate to the project directory:
    ```sh
    cd house-price-prediction
    ```
3. Install the required libraries:
    ```sh
    pip install -r requirements.txt
    ```
4. Run the jupyter notebook :
    ```sh
    jupyter notebook
    ```
5. Select Project file :
   ```sh
    select > project.ipynb
    ```

## Dependencies

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## Results

The script prints the R-squared score of the linear regression model on the test data, both for the simple linear model and the polynomial features model.

