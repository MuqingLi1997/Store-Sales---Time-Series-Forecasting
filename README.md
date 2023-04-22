# Store-Sales---Time-Series-Forecasting
# **Store Sales - Time Series Forecasting**

Use machine learning to predict grocery sales

## **Goal of the Competition**

In this “getting started” competition, you’ll use time-series forecasting to forecast store sales on data from Corporación Favorita, a large Ecuadorian-based grocery retailer.

Specifically, you'll build a model that more accurately predicts the unit sales for thousands of items sold at different Favorita stores. You'll practice your machine learning skills with an approachable training dataset of dates, store, and item information, promotions, and unit sales.

The evaluation metric for this competition is **Root Mean Squared Logarithmic Error**.

The **RMSLE** is calculated as:

$$
[\sqrt{ \frac{1}{n} \sum_{i=1}^n \left(\log (1 + \hat{y}_i) - \log (1 + y_i)\right)^2}]
$$

where:

- 𝑛 is the total number of instances,
- 𝑦̂ 𝑖 is the predicted value of the target for instance (i),
- 𝑦𝑖 is the actual value of the target for instance (i), and,
- log is the natural logarithm.

## **Submission File**

For each **id** in the test set, you must predict a value for the **sales** variable. The file should contain a header and have the following format:


# **Dataset Description**

In this competition, you will predict sales for the thousands of product families sold at Favorita stores located in Ecuador. The training data includes dates, store and product information, whether that item was being promoted, as well as the sales numbers. Additional files include supplementary information that may be useful in building your models.

### **train.csv**

- The training data, comprising time series of features **store_nbr**, **family**, and **onpromotion** as well as the target **sales**.
- **store_nbr** identifies the store at which the products are sold.
- **family** identifies the type of product sold.
- **sales** gives the total sales for a product family at a particular store at a given date. Fractional values are possible since products can be sold in fractional units (1.5 kg of cheese, for instance, as opposed to 1 bag of chips).
- **onpromotion** gives the total number of items in a product family that were being promoted at a store at a given date

### **test.csv**

- The test data, having the same features as the training data. You will predict the target **sales** for the dates in this file.
- The dates in the test data are for the 15 days after the last date in the training data.

### **sample_submission.csv**

- A sample submission file in the correct format.

### **stores.csv**

- Store metadata, including **city**, **state**, **type**, and **cluster**.
- **cluster** is a grouping of similar stores.

### **oil.csv**

- Daily oil price. Includes values during both the train and test data timeframes. (Ecuador is an oil-dependent country and it's economical health is highly vulnerable to shocks in oil prices.)

### **holidays_events.csv**

- Holidays and Events, with metadata
- NOTE: Pay
