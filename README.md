# 📊 Sales Revenue Prediction Using RNN

## 📌 Project Overview

This project focuses on predicting next-day sales revenue using Deep Learning techniques, particularly **Recurrent Neural Network (RNN)**.

The model analyzes historical sales data, store information, and product categories to predict future sales revenue.

It uses time-series sequence modeling to learn patterns from the previous 10 records and predict the next record's revenue.

## 🎯 Project Objectives

- Predict next-day sales revenue using Deep Learning.
- Analyze historical sales revenue patterns.
- Understand time-series forecasting using RNN.
- Preprocess and normalize sales data.
- Train and evaluate an RNN model.
- Visualize actual vs predicted sales revenue.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- TensorFlow / Keras
- Jupyter Notebook / Google Colab

## 📂 Dataset Description

The project uses a sales revenue dataset named `sales_revenue_dataset.csv`.

### Dataset Features

| Feature | Description |
|---|---|
| Date | Sales transaction date |
| Store_ID | Store identification |
| Product_Category | Product category |
| Revenue | Sales revenue (Target Variable) |

The dataset also uses its available numerical features during model training.

## ⚙️ Project Workflow

1. Import the required Python libraries.
2. Upload and load the sales revenue dataset.
3. Analyze dataset shape and revenue statistics.
4. Remove the Date column.
5. Encode categorical features using LabelEncoder.
6. Normalize the data using MinMaxScaler.
7. Create time-series sequences using the previous 10 records.
8. Split the dataset into 80% training and 20% testing.
9. Build a Recurrent Neural Network model.
10. Train the model using Early Stopping.
11. Predict sales revenue.
12. Evaluate model performance.
13. Visualize actual vs predicted revenue.

## 🧠 Deep Learning Model

**Recurrent Neural Network (Simple RNN)**

The project uses the following RNN architecture:

- SimpleRNN – 64 units (return_sequences=True)
- Dropout – 0.2
- SimpleRNN – 32 units
- Dropout – 0.2
- Dense Layer – 16 neurons (ReLU activation)
- Output Layer – 1 neuron

### Model Configuration

- Optimizer: Adam
- Learning Rate: 0.001
- Loss Function: Mean Squared Error (MSE)
- Batch Size: 16
- Maximum Epochs: 100
- Early Stopping: Patience = 15
- Activation Function: Tanh (RNN layers)

## 📈 Model Evaluation

The model performance is evaluated using:

- **MAE (Mean Absolute Error):** Measures the average absolute difference between actual and predicted revenue.
- **RMSE (Root Mean Squared Error):** Measures prediction errors while giving more weight to larger errors.
- **R² Score:** Measures how well the model explains variations in sales revenue.

## 📉 Data Visualization

The project includes four visualizations:

1. **Training vs Validation Loss:** Displays model training performance.
2. **Actual vs Predicted Revenue:** Compares actual and predicted sales revenue.
3. **Actual vs Predicted Scatter Plot:** Visualizes prediction accuracy.
4. **Category-Wise Revenue Bar Chart:** Displays average revenue by product category.

## 🚀 How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/Sales-Revenue-Prediction-RNN.git
```

### 2. Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn tensorflow jupyter
```

### 3. Open Jupyter Notebook

```bash
jupyter notebook
```

### 4. Run the Notebook

Open `SALES_REVENUE_PREDICTION_USING_RNN.ipynb` and execute all cells.

### 5. Upload Dataset

Upload the required dataset:

`sales_revenue_dataset (1).csv`

Make sure the dataset is available at the path expected by the notebook.

## 📁 Project Structure

```text
Sales-Revenue-Prediction-RNN/
│
├── SALES_REVENUE_PREDICTION_USING_RNN.ipynb
├── sales_revenue_dataset.csv
├── Rnn Sales Charts.png
└── README.md
```

## 🔮 Future Enhancements

- Experiment with LSTM and GRU models.
- Improve prediction accuracy through hyperparameter tuning.
- Include additional sales-related features.
- Develop an interactive sales prediction dashboard using Streamlit.
- Integrate real-time sales data.
- Compare different Deep Learning algorithms.

## ⚠️ Disclaimer

This project is developed for educational and academic purposes only. Predicted sales revenue values are model estimates and may differ from actual business revenue.

## 👨‍💻 Author

**Mohamed Aziz**

Deep Learning Project – Sales Revenue Prediction Using RNN.

---

⭐ If you find this project useful, don't forget to star the repository!
