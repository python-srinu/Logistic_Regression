# Handwritten Digits Classification with Logistic Regression

This project uses **Logistic Regression** to classify handwritten digits (0-9) from the **Digits dataset** in `sklearn`. It includes data preparation, model training, evaluation, and visualization.

---

## Project Highlights
- Visualizes sample images from the dataset.
- Prepares the data for machine learning models.
- Tunes hyperparameters using **GridSearchCV**.
- Compares training and testing accuracy for different test sizes.
- Displays a **confusion matrix** to show classification results.
- Allows testing predictions on individual images.

---

## Dataset Overview
The dataset contains:
- **Images**: Grayscale images of size 8x8 pixels.
- **Labels**: Numbers from 0 to 9.

### Sample Images

Here are some examples of the digits in the dataset:

| Sample Images | Labels |
|---------------|--------|
| ![Digit Example](https://via.placeholder.com/80?text=0) ![Digit Example](https://via.placeholder.com/80?text=1) ![Digit Example](https://via.placeholder.com/80?text=2) ![Digit Example](https://via.placeholder.com/80?text=3) ![Digit Example](https://via.placeholder.com/80?text=4) |

---

## Steps in the Project

1. **Data Splitting**  
   The data is split into training and testing sets with different **test sizes** (`0.2` and `0.3`) to analyze how the split affects model performance.

2. **Hyperparameter Tuning**  
   The best settings for the model are found using **GridSearchCV**, which tests different:
   - Regularization (`l1`, `l2`, etc.)
   - Solvers (`lbfgs`, `liblinear`, etc.)
   - Regularization strength (`C` values like 0.1, 1, 10, 100)
   - Maximum iterations (100, 500, 1000)

3. **Model Training and Evaluation**  
   The model is trained with the best hyperparameters, and the accuracy is checked on both training and testing data.

4. **Performance Visualization**  
   A **confusion matrix** is plotted to show how well the model predicts each digit.

5. **Prediction Testing**  
   You can test the model by predicting any sample image and comparing the prediction with the actual label.

---

## Results

### Accuracy Summary
| Test Size | Train Accuracy | Test Accuracy |
|-----------|----------------|---------------|
| 0.2       | 0.98         | 0.96        |
| 0.3       | 1.00          | 0.97         |

- **Best Test Size**: `0.3`
- **Highest Accuracy**: `0.97`

---

## Visualizations

### Confusion Matrix  
The confusion matrix shows how accurately the model predicts each digit. This helps identify which digits the model struggles with.

### Sample Image Prediction  
You can select any test image to see:
- **True Label**: The actual digit.
- **Predicted Label**: What the model predicted.

---

## Tools Used

- **Python**: Programming language
- **Libraries**:
  - `numpy` for data processing
  - `matplotlib` for visualization
  - `sklearn` for dataset, model training, and evaluation

---

## How to Run the Code

1. Download the code from this repository.
2. Install the required libraries:  
   ```bash
   pip install numpy matplotlib scikit-learn
3. Run the script in your Python environment.
4. Explore the results and test the model with sample images.

---

### Why This Project?

This project is a great example of:

- Working with real-world data.
- Using machine learning techniques like logistic regression and hyperparameter tuning.
- Visualizing and analyzing model performance.
