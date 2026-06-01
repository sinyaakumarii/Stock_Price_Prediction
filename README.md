# Stock Price Prediction using Linear Regression

An end-to-end Machine Learning pipeline implemented in a Jupyter Notebook to predict stock closing prices using historical data. The project utilizes structural data preprocessing techniques, scaling, and a Scikit-Learn Linear Regression model.

---

## 💻 Project Workflow

1. **Data Loading & Preprocessing:** Handles missing values via forward-filling (`ffill`), converts date formats, and sorts chronological timelines.
2. **Feature Scaling:** Implements `MinMaxScaler` to normalize input metrics.
3. **Data Splitting:** Uses a chronological split (80% training, 20% testing) to preserve real-world stock market timelines.
4. **Model Training:** Fits a `LinearRegression` model using the parameters: `Open`, `High`, `Low`, and `Volume`.
5. **Evaluation:** Measures performance using Mean Squared Error (MSE) and the $R^2$ Score.

---

## 📊 Dataset Structure

The model expects a `StockPriceDataset.csv` containing the following attributes:
* `Date`: The historical date of trading.
* `Open`: The starting price of the stock for the day.
* `High`: The highest price reached during the session.
* `Low`: The lowest price dropped to during the session.
* `Close`: The final trading price (Target Variable).
* `Volume`: Total number of shares traded.
* `Ticker`: Stock symbol identifiers (e.g., AAPL, AMZN, GS).

---

## 📈 Model Performance

The current configuration yields the following metrics on the test dataset:

| Evaluation Metric | Score |
| :--- | :--- |
| **Mean Squared Error (MSE)** | `1.4594` |
| **$R^2$ Score (Coefficient of Determination)** | `0.9997` |

---

## 🛠️ Setup Instructions

### Prerequisites
Make sure you have Python 3.8+ installed.

### 1. Clone the Repository
```bash
git clone [https://github.com/your-username/your-repo-name.git](https://github.com/sinyaakumarii/Stock_price_prediction.git)