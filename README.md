# Hotel Cancellation Prediction using Deep Learning

A deep learning project focused on predicting hotel booking cancellations using customer and reservation data.

This project was developed as part of a university deep learning final assignment and demonstrates the application of neural networks to solve a real-world business problem in the hospitality industry.

---

# Business Problem

Hotel booking cancellations create major financial and operational challenges for hotels, including:

- Revenue loss
- Poor room occupancy planning
- Inefficient resource allocation
- Increased operational uncertainty

The goal of this project is to build a neural network capable of predicting whether a hotel reservation will be canceled before arrival.

Such predictions can help hotels:

- Improve revenue management
- Optimize booking strategies
- Reduce cancellation-related losses
- Support business decision-making

---

# Dataset

The project uses the Hotel Booking Demand Dataset, which contains information about hotel reservations including:

- Lead time
- Customer type
- Deposit type
- Meal plan
- Market segment
- Number of guests
- ADR (Average Daily Rate)
- Previous cancellations
- Special requests
- And more

Target variable:

```python
is_canceled
```
- 0 → Booking not canceled
- 1 → Booking canceled


# Technologies Used
- Python
- TensorFlow / Keras
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Machine Learning Pipeline

The project follows a complete machine learning workflow:

- Data preprocessing
- Missing value handling
- Feature scaling
- One-hot encoding
- Train-validation split
- Neural network training
- Model evaluation
- Performance visualization

# Neural Network Architecture

The model architecture includes:

- Batch Normalization
- Dense Layers
- ReLU activation
- Dropout regularization
- Sigmoid output layer

Architecture summary:
```python

    BatchNormalization
    Dense(256, relu)
    BatchNormalization
    Dropout(0.3)
    Dense(256, relu)
    BatchNormalization
    Dropout(0.3)
    Dense(1, sigmoid)
```

# Model Performance

Final validation accuracy:

~84%

Evaluation metrics included:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

The model achieved strong performance in predicting hotel booking cancellations while maintaining balanced generalization on validation data.

# Repository Structure
hotel-cancellation-prediction-dl/
│
├── data/
├── images/
├── notebook/
│   └── hotel_cancellation_prediction.ipynb
├── presentation/
├── README.md
├── requirements.txt
└── .gitignore

# Future Improvements

Possible future improvements include:

- Hyperparameter tuning
- Model deployment with Streamlit or Flask
- Explainable AI techniques
- Feature importance analysis
- Trying advanced architectures
- Handling class imbalance more effectively

# Results

## Neural Network Architecture

  ![Architecture](images/neural_network_architecture.png)

## Accuracy Curve

  ![Accuracy Curve](images/accuracy_curve.jpg)

## Loss Curve

  ![Loss Curve](images/loss_curve.jpg)

## Confusion Matrix

  ![Confusion Matrix](images/confusion_matrix.jpg)

# Author

Ghazal Koobchi

Computer Science Graduate | Deep Learning & Data Science Enthusiast