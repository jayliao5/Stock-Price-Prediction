# Stock-Price-Prediction Using Stacked LSTM

## Team Members
- Yitian Wang
- Zhixuan Li
- Jason Liao
- Sihan Zhou
- Mia Kwon

## Project Overview
This project focuses on predicting stock prices using a Stacked LSTM model, a critical challenge in financial markets due to the inherent volatility and trend patterns of stock data. Our model targets historical stock prices of Goldman Sachs (GS) from 2011 to 2023, leveraging data like Open, High, Low, Close prices, and Volume of stocks traded.

## Relevance and Business Impact
The application of our Stacked LSTM model can revolutionize various aspects of the financial sector by enabling informed and profitable investment strategies, enhancing financial stability, improving investor confidence, and supporting regulatory compliance. Key benefits include:
- **Improved Decision Making:** Offers a data-driven approach, reducing reliance on speculative methods.
- **Increased ROI:** Facilitates entering and exiting positions at optimal times.
- **Risk Mitigation:** Helps in early identification of negative trends, thus protecting investments.
- **Competitive Advantage:** Provides an edge over competitors by utilizing advanced predictive tools.

## Data Preparation and Preprocessing
Data preparation involved normalization using MinMaxScaler to scale features between 0 and 1, ensuring uniformity and aiding in the model's training efficiency. The data was then formatted into sequences using a defined lookback period of 30 days, suitable for LSTM which learns from historical dependencies to predict future stock prices.

## Model Architecture
The Stacked LSTM model was chosen over standard LSTM due to its ability to capture complex relationships and long-term dependencies crucial for stock price prediction. The model includes several LSTM layers followed by a fully connected layer to map the output of the LSTM layers to the desired output shape. Hyperparameters like hidden dimensions, number of layers, learning rate, dropout rate, and weight decay were carefully tuned to optimize the model.

## Implementation and Challenges
Implemented in a Jupyter notebook, the project involves:
- Data loading and preprocessing.
- Defining the LSTM model structure.
- Model training and evaluation.
- Hyperparameter tuning using Hyperopt.

Challenges addressed included managing model complexity and leveraging GPU acceleration for training.

## Results and Evaluation
The model's effectiveness was assessed using RMSE and visual analysis of predictions vs. actual stock prices. It achieved a training RMSE of 5.00 and a testing RMSE of 10.90, significantly outperforming an XGBoost benchmark.

## Deployment
The deployment strategy can be adapted to either cloud-based environments for scalability and accessibility or on-premise for enhanced security. Integration into existing trading platforms could allow real-time decision-making based on the model’s insights.

## Ethical and Risk Considerations
The model's deployment considers ethical transparency, acknowledgment of market unpredictability, and prevention against potential misuse for market manipulation.

## Contributions
Each team member contributed equally to the project, ensuring a collaborative effort throughout the project's phases.

---

For more details on the implementation, refer to the Jupyter notebooks and scripts provided in this repository.
