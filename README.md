# Deep Learning Practical Assignment

## Q6. Dataset Augmentation

- **Task:**  
  Use `sklearn.datasets.make_moons()` to generate a 2D dataset.
- **Augmentation:**  
  - Add Gaussian noise to the data  
  - Flip some points horizontally
- **Visualization:**  
  Plot original vs augmented dataset side by side.
- **Explanation:**  
  Discuss why data augmentation helps reduce overfitting.

---

## Q7. Dropout Experiment

- **Task:**  
  Build a 2-hidden-layer MLP using PyTorch/Keras on the Q6 dataset (or MNIST subset).
- **Experiments:**  
  - Train with dropout (`p=0.5`)  
  - Train without dropout
- **Visualization:**  
  Plot training & validation loss curves for both.
- **Analysis:**  
  Explain which model generalizes better and why.

---

## Q8. Batch Normalization in MLP

- **Task:**  
  Modify the same MLP by adding Batch Normalization after each hidden layer.
- **Experiments:**  
  - Train with BatchNorm  
  - Train without BatchNorm
- **Comparison:**  
  Compare convergence speed (epochs to reach 90% training accuracy).
- **Discussion:**  
  Discuss how BatchNorm stabilizes training.

---

## Q9. Hyperparameter Tuning with k-Fold Cross-Validation

- **Task:**  
  Train an MLP with 3 different hidden layer sizes: `[16, 8, 1]`, `[32, 16, 1]`, `[64, 32, 1]`.
- **Validation:**  
  Use 5-fold cross-validation to select the architecture with the highest mean validation accuracy.
- **Output:**  
  Print the mean accuracy for each architecture and the best one.

---

## Q10. Regularization (Parameter Norm Penalty)

- **Task:**  
  Train an MLP with and without L2 regularization on the same dataset.
- **Comparison:**  
  Compare final training loss and validation loss.
- **Analysis:**  
  Show how regularization prevents overfitting by keeping weights small (print average weight norm).

---

**Each question is implemented in its own Jupyter notebook inside the corresponding folder (Q6, Q7, Q8, Q9, Q10).**