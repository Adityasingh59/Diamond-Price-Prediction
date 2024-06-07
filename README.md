# Diamond-Price-Prediction


![Diamonds](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRYXxvva3ik29uwZu8mFw1c0NQ3LLp652C7tti2zT6l3WtvZNVgwFpUf9oNbIVefipZb-4&usqp=CAU)

## Project Overview

Welcome to my Diamonds Price Prediction project! In this project, I tackled the challenge of determining an optimal bid price for a jewelry company interested in purchasing a large set of diamonds at an auction. Using a linear regression model, I created a recommendation on how much the company should bid for these diamonds.

## Project Details

A diamond distributor has recently decided to exit the market and has put up 3,000 diamonds for auction. Recognizing a prime opportunity to expand their inventory, a jewelry company seeks to place a competitive bid. To assist in this decision, I used a linear regression model based on an extensive database of diamond prices to predict the price of each diamond in the auction set.

The regression equation used is as follows:

\[ \text{Price} = -5269 + 8413 \times \text{Carat} + 158.1 \times \text{Cut} + 454 \times \text{Clarity} \]

## Steps Taken

### Step 1 – Understand the Data

There are two key datasets used in this project:

- **[diamonds.csv](./diamonds.csv)**: This dataset was used to build the regression model and contains carat, cut, clarity, and price information.
- **[new_diamonds.csv](./new_diamonds.csv)**: This dataset includes the carat, cut, and clarity details for the diamonds the company aims to purchase.

**Variable Descriptions:**

- **Carat**: Represents the weight of the diamond (numerical).
- **Cut**: Quality of the diamond cut, categorized into 5 levels (fair, good, very good, ideal, premium), represented as 1-5 in `Cut_Ord`.
- **Clarity**: Internal purity of the diamond, categorized into 8 levels (I1, SI2, SI1, VS1, VS2, VVS2, VVS1, IF), represented as 1-8 in `Clarity_Ord`.

> Note: Ordinal transformation of categorical variables is used here for simplicity.

### Step 2 – Calculate the Predicted Price for Diamonds

For each diamond in the `new_diamonds.csv` dataset, I used the regression equation to predict its price. This involved:

- **Loading the datasets**: Read and preprocess data from `diamonds.csv` and `new_diamonds.csv`.
- **Encoding categorical variables**: Convert categorical variables into numerical format using label encoding.
- **Training the model**: Train a linear regression model on the `diamonds.csv` data.
- **Predicting prices**: Apply the trained model to predict prices for diamonds in `new_diamonds.csv`.

### Step 3 – Make a Recommendation

Using the model predictions, I calculated the total retail price of the diamonds. To determine a suitable bid, the company should consider purchasing the diamonds at 70% of this total predicted price, as this reflects the typical purchase price from distributors.

## Data

The following data files are used in the project:

- **[diamonds.csv](./diamonds.csv)**: Contains carat, cut, clarity, and price information for each diamond in the dataset used to build the regression model.
- **[new_diamonds.csv](./new_diamonds.csv)**: Contains carat, cut, and clarity information for the diamonds the company would like to purchase.

## Results and Conclusion

The linear regression model effectively predicted the prices of the diamonds, and the final recommendation for the bid price was calculated by taking 70% of the total predicted retail price. This approach provides a strategic advantage by ensuring the company bids a fair price aligned with the predicted market value.

### Key Takeaways:

- **Data Understanding**: Effectively understanding the features of the dataset is crucial for accurate predictions.
- **Feature Encoding**: Proper encoding of categorical variables is essential for model training.
- **Model Training and Prediction**: Linear regression can be a powerful tool for predicting diamond prices when feature relationships are well-understood.
- **Bid Recommendation**: The final bid recommendation is based on a calculated percentage of the predicted retail price to align with typical purchasing practices.

## Contact

For questions or further information, feel free to reach out:

- **Aditya Singh**
- [Email](mailto:singhadit.509@gmail.com)
- 
