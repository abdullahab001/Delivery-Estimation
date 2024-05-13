# Delivery Time Estimation
 
One of the India's Largest Marketplace for Intra-City Logistics. Leader in the country's $40 billion intra-city logistics market, it strives to improve the lives of 1,50,000+ driver-partners by providing them with consistent earning & independence. Currently, the company has serviced 5+ million customers

This company works with a wide range of restaurants for delivering their items directly to the people.

It has a number of delivery partners available for delivering the food, from various restaurants and wants to get an estimated delivery time that it can provide the customers on the basis of what they are ordering, from where and also the delivery partners.

# Solution Approach
To address this challenge, we leveraged the power of Neural Networks (NN) to build a delivery time estimation model. Our model takes into account various factors such as the ordered time, pickup location, delivery time, and available delivery partners to predict the estimated delivery time accurately.

# Data Collection and Preprocessing
We have historical order data including features such as `market_id`, `store_id`, `store_primary_category`, `order_protocol`, `total_items`, `subtotal`, `num_distinct_items`, `min_item_price`, `max_item_price`, `total_onshift_partners`, `total_busy_partners`, `total_outstanding_orders`. Additionally, we calculated hour of the day, day of week the delivery_time in minutes as our target variable.

We preprocessed the data by handling missing values, encoding categorical variables, and scaling numerical features to ensure faster convergence with the neural network model.

# Model Architecture
Our neural network model consists of multiple dense layers with ReLU activation functions. We used the Adam optimizer, Glorot uniform kernel initializer  and Mean Squared Error loss function for training. 

# Training and Evaluation
We split the data into training, validation, and test sets and trained the model on the training data. We evaluated the model's performance on the validation set and fine-tuned the hyperparameters to improve performance.

# Results
Our model achieved impressive results with below mentioned metrics on the test set. 

Mean Squared Error: 175.83023181375756
Root Mean Squared Error: 13.260099238458118
Mean Absolute Error: 10.295266447127483
R2 Score: 0.3357127483 (Feature correlation with the delivery time is very low, we should consider including more relevant features.)

The estimated delivery time provided by our model has significantly improved the delivery estimates.
