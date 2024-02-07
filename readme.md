# Zumi Obstacle Classification
A Machine Learning project written with Python in Jupyter Notebook to instruct Zumi to classify two objects using the k-NN and Logistic Regression algorithms. 

**Zumi Website:** https://www.robolink.com/products/zumi

This project trains Zumi with a `soft toy` and `plastic cup`. 

[**Download all files**](https://github.com/sidneyshafer/zumi-project/archive/refs/heads/main.zip) (including pickled data files) and follow instructions in the Juypter Notebook file (`zumi-final-code.ipynb`)

## `zumi-final-code` Jupyter Notebook Details

### Classifying Objects Using Pickled Data Files
The project can be run two different ways to classify objects:
1. Classify obstacles *without* noise
2. Classify obstacles **with noise**

### 1. <ins>Classify obstacles *without* noise</ins>
1. Under **Data Collection**, run the first cell of code.
   ![image](https://github.com/sidneyshafer/zumi-project/assets/66838571/a711c8b1-e35a-4af6-8f63-95ae0714116c)

2. Run the second cell of code.
  ![image](https://github.com/sidneyshafer/zumi-project/assets/66838571/dc3385ea-7271-46aa-959c-f8eda189b2ca)

3. Under **Data Collection - *collect data without noise***, run the first cell.
   ![image](https://github.com/sidneyshafer/zumi-project/assets/66838571/f55c65e2-4668-47cb-9420-e507d72d3fe4)

4. <ins>DO NOT</ins> run the cells under **Data Augmentation - *collect data with noise***.
5. Under **Storing & Visualizing Data**, run the first cell to visualize the data points.
   ![image](https://github.com/sidneyshafer/zumi-project/assets/66838571/e6a504c6-c6d2-437d-b18c-70ca1a290e6c)

6. Under **Plotting Data**, run both cells to visualize the data on a 2D and 3D graph.
7. Under **Implementing & Training k-NN and Logistic Regression**, run both code cells to train the machine learning models.
8. Run the code cell under **Hyperparameter Tuning** to determine the best value for `k`.
9. Run the code cell under **Confusion Matrix** to generate a confusion matrix for each model.
10. Under **Cross-Validation with cross_val_score**, run the cell to implement k-fold cross validation.
11. The section under **Real-time Decision Making** allows Zumi to react in real-time to a classified object.

    a. Place Zumi in front of an object (i.e. a soft toy, plastic cup, or any other object you wish to classify).

    b. Run the first cell to define the `react_to_obstacle` function.

    c. Run the second cell to define the `classify_obstacle` function - this function will classify the object.
    
12. Run the cell under **Evaluation** to check the accuracy of the k-NN and Logistic Regression models.

### 2. <ins>Classify obstacles **with noise**</ins>
1. Under **Data Collection**, run the first and second cells of code.
2. <ins>DO NOT</ins> run the cells under **Data Collection - *collect data without noise***.
3. Only run the first cell under **Data Augmentation - *collect data with noise***. <ins>DO NOT</ins> run the second cell.
   ![image](https://github.com/sidneyshafer/zumi-project/assets/66838571/a2f01018-c9f4-4316-b0c6-9a3913eb2d09)

4. Under **Storing & Visualizing Data**, run the first cell to visualize the data points.
5. Under **Plotting Data**, run both cells to visualize the data on a 2D and 3D graph.
6. Under **Implementing & Training k-NN and Logistic Regression**, run both code cells to train the machine learning models.
7. Run the code cell under **Hyperparameter Tuning** to determine the best value for `k`.
8. Run the code cell under **Confusion Matrix** to generate a confusion matrix for each model.
9. Under **Cross-Validation with cross_val_score**, run the cell to implement k-fold cross validation.
10. The section under **Real-time Decision Making** allows Zumi to react in real-time to a classified object.

    a. Place Zumi in front of an object (i.e. a soft toy, plastic cup, or any other object you wish to classify).

    b. Run the first cell to define the `react_to_obstacle` function.

    c. Run the second cell to define the `classify_obstacle` function - this function will classify the object.
    
11. Run the cell under **Evaluation** to check the accuracy of the k-NN and Logistic Regression models.

### Data Collection
**NOTE: You will need a fully operational Zumi to gather sensor reading data for this section.**

The project can be run two different ways to collect data points for classifying objects:
1. Collect data points *without* adding noise.
2. Collect data points with augmentation (add noise).

### 1. <ins>Collect data points *without* adding noise</ins>
1. Under **Data Collection**, run the first and second cells of code.
2. Under **Data Collection - *collect data without noise***, run the first cell of code.
3. <ins>DO NOT</ins> run the *first* cell under **Data Augmentation - *collect data with noise***.
4. ONLY Run the second cell and follow the instructions:

   **NOTE:** Place Zumi in front of an obstacle (either a `soft toy` or `plastic cup`) to collect sensor readings.
   ![image](https://github.com/sidneyshafer/zumi-project/assets/66838571/54f48bc7-97fc-4cbd-82df-bb3c241822ec)

5. Repeat Step 4 until you have the desired amount of data points.
6. After Data Collection is complete, execute the rest of the code cells in the notebook (as described in the sections above).

### 2. <ins>Collect data points with augmentation (add noise)</ins>
1. Under **Data Collection**, run the first and second cells of code.
2. <ins>DO NOT</ins> run the cell under **Data Collection - *collect data without noise***.
3. Run the first cell under **Data Augmentation - *collect data with noise***.

   a. This code opens the `zumi_data_noise.pkl` file.
   ![image](https://github.com/sidneyshafer/zumi-project/assets/66838571/fd999540-7910-43f9-9f8b-ccf70b4d8771)

4. Then, run the second cell and follow the instructions:

   **NOTE:** Place Zumi in front of an obstacle (either a `soft toy` or `plastic cup`) to collect sensor readings.
   ![image](https://github.com/sidneyshafer/zumi-project/assets/66838571/54f48bc7-97fc-4cbd-82df-bb3c241822ec)

5. Repeat Step 4 until you have the desired amount of data points.
7. After Data Collection is complete, execute the rest of the code cells in the notebook (as described in the sections above).
