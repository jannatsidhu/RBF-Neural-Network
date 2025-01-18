# RBF Neural Network for Function Approximation

This project implements a Radial Basis Function (RBF) Neural Network to approximate a mapping function defined by the equation:

f(x1, x2) = +1 if (x1^2 + x2^2 <= 1) and -1 if (x1^2 + x2^2 > 1).

## Dataset Description
- **Points Generated:** 441 points, defined as:
  
  x = (x1, x2) where x1 = -2 + 0.2 * i (where i = 0, 1, .... 20) and x2 = -2 + 0.2 * j (where j = 0, 1, .... 20)
- **Train/Test Split:** 
  - Training set: 80% of points
  - Test set: 20% of points

## Methodology

### Scenarios for Centers of Radial Basis (RB) Functions:
1. **All Training Points as Centers:**
   - Each training point serves as a center for the RB functions.

2. **150 Points as Centers:**
   - **Random Selection:** 150 centers are randomly selected from the training data.
   - **KMeans Clustering:** 150 centers are chosen using KMeans clustering to group the training data points effectively.

### Steps:
1. **Data Preparation:** Generate points and split them into training and test sets.
2. **Model Implementation:** Design an RBF Neural Network.
3. **Evaluation:** Compare the performance across different scenarios and methods of center selection.

## Technologies Used
- **Programming Language:** Python
- **Libraries:**
  - NumPy: For numerical computations.
  - Matplotlib: For visualizations.
  - Scikit-learn: For KMeans clustering.

## Key Features
- Implementation from scratch of an RBF Neural Network.
- Function approximation based on a geometric classification task.
- Comparison of methods to determine RB function centers.

## Results
The performance of the RBF network is evaluated based on accuracy and the ability to correctly classify the test points for each scenario.

## Instructions to Run
1. Install required libraries: `numpy`, `matplotlib`, `sklearn`.
2. Clone or download this repository.
3. Run the provided Jupyter notebook to view the implementation and results.

## Example Visualization
The final output includes plots demonstrating the classification of the 441 points and the decision boundary of the RBF Neural Network.

---

This implementation explores the effectiveness of RBF Neural Networks in solving a fundamental classification task and highlights the impact of different center selection strategies.

