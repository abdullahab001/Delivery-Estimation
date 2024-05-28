# Optimizing Porter Delivery Estimates

**Project Overview**

Our project focused on optimizing delivery estimates for Porter, a leading marketplace in India's intra-city logistics sector. With a commitment to enhancing the livelihoods of over 150,000 driver-partners and serving more than 5 million customers, Porter sought to provide accurate delivery time estimates based on various factors such as order details, pickup location, and available delivery partners.

**Solution Approach**

To meet this challenge, we employed advanced Neural Networks (NN) to develop a delivery time estimation model. Our model incorporated key features including ordered time, pickup location, delivery time, and available delivery partners to predict delivery estimates accurately.

**Data Collection and Preprocessing**

Our dataset comprised historical order data with features such as market_id, store_id, order_protocol, total_items, and more. We preprocessed the data by handling missing values, encoding categorical variables, and scaling numerical features, ensuring optimal convergence with the neural network model.

**Model Architecture**

The neural network model consisted of multiple dense layers with ReLU activation functions. We utilized the Adam optimizer, Glorot uniform kernel initializer, and Mean Squared Error loss function for training.

**Training and Evaluation**

After splitting the data into training, validation, and test sets, we trained the model on the training data. Evaluation on the validation set allowed us to fine-tune hyperparameters, optimizing model performance.

**Results and Recommendations**

Our model achieved impressive results on the test set, with Mean Squared Error, Root Mean Squared Error, Mean Absolute Error, and R2 Score metrics indicating significant improvement in delivery time estimation accuracy.

**Actionable Insights & Recommendations**

1. **Feature Expansion** Considering the low feature correlation with delivery time, we recommend including additional relevant features in future iterations to enhance model performance further.

2. **Continuous Improvement** Regular model updates and retraining with fresh data will be essential to ensure ongoing accuracy and relevance in delivery time estimation.

By leveraging these insights and recommendations, Porter can continue to enhance its delivery estimation accuracy, ultimately improving customer satisfaction and operational efficiency.
