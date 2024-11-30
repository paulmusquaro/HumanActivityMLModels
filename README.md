# HumanActivityMLModels

This project focuses on classifying human activity data based on accelerometer measurements using three different machine learning models: Support Vector Machine (SVM) with a linear kernel, Support Vector Machine with a Radial Basis Function (RBF) kernel, and Random Forest Classifier.

## The Results of Three Models:

1. **Support Vector Machine (SVM) with Linear Kernel:**
   - **Performance**: The model achieves outstanding accuracy, with 0.996 on the training set and 0.997 on the test set, indicating near-perfect performance on both datasets.
   - **Metrics**: Precision, recall, and F1-score values approach 1.0 for all classes, demonstrating the model’s effectiveness in distinguishing between the activity classes (idle, running, walking, stairs).
   - **Recommendation**: The linear SVM is highly accurate and generalizes well to new data, making it an excellent choice for this classification task.

2. **Support Vector Machine (SVM) with Radial Basis Function (RBF) Kernel:**
   - **Performance**: Accuracy is 0.977 on the training set and 0.968 on the test set, which is lower than the linear kernel model but still respectable.
   - **Metrics**: While precision and recall are strong for the idle and running classes, the model struggles with the walking class, showing low recall and F1-score. The stairs class is better, though still not as strong as the linear SVM.
   - **Recommendation**: The RBF SVM performs well overall, but it faces challenges with class imbalances. It may need additional tuning or resampling techniques to improve performance on underrepresented classes.

3. **Random Forest Classifier:**
   - **Performance**: The Random Forest classifier achieves perfect accuracy (1.0) on both the training and test sets.
   - **Metrics**: Precision, recall, and F1-score are all 1.0 for each class, showing flawless classification with no misclassifications.
   - **Recommendation**: Random Forest is the top-performing model in this project. It excels at handling class imbalances and provides robust performance across all metrics, making it the best choice for this task.



## Conda (Setup and Environment)

To make the project reproducible and ensure smooth package management, this project uses Conda as a package and environment manager. Below are the steps to set up the environment:


1. **Install Conda**:
If you haven't installed Conda yet, you can download it from the official [Anaconda](https://www.anaconda.com/products/individual) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html) websites. Anaconda is a larger distribution with more pre-installed packages, while Miniconda is a smaller, minimal version. Choose whichever suits your needs.

2. **Create a new environment:** Open your terminal and run the following command to create a new Conda environment with Python 3.12:

    ```bash
    conda create --name new_conda_env python=3.12
    ```

3. **Activate the environment:** Once the environment is created, activate it by running:

    ```bash
    conda activate new_conda_env
    ```

4. **Install required packages (Jupyter, NumPy, Pandas and Scikit-Learn)**

    ```bash
    conda install jupyter numpy pandas scikit-learn
    ```

5. **Run Jupyter Notebook**

    ```bash
    jupyter notebook
    ```

***
## Conclusion

This analysis highlights the effectiveness of Random Forest for activity classification, though Linear SVM remains a strong alternative for simpler, interpretable models.