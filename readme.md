# Zumi Obstacle Classification
A Machine Learning project written with Python in Jupyter Notebook to instruct Zumi to classify two objects using the k-NN and Logistic Regression algorithms. 

**Zumi Website:** https://www.robolink.com/products/zumi

This project trains Zumi with a `soft toy` and `plastic cup`. 
Download **all** files (including pickled data files) and follow instructions in the Juypter Notebook file (zumi-final-code.ipynb)

## `zumi-final-code` Jupyter Notebook Details

### Classifying Objects Using Pickled Data
This project can be run two different ways to classify objects:
1. Classify objects using data points *without* noise.
2. Classify objects using data **with noise**.

#### Classify Obstacles Without Noise
1. Under **"Data Collection"**, run the first cell of code.
   ![image](https://github.com/sidneyshafer/zumi-project/assets/66838571/a711c8b1-e35a-4af6-8f63-95ae0714116c)

2. Run the second cell of code.
  ![image](https://github.com/sidneyshafer/zumi-project/assets/66838571/dc3385ea-7271-46aa-959c-f8eda189b2ca)

3. under **"Data Collection - *collect data without noise*"**, run the first cell.
   ![image](https://github.com/sidneyshafer/zumi-project/assets/66838571/f55c65e2-4668-47cb-9420-e507d72d3fe4)

4. DO NOT run the cells under **"Data Augmentation - *collect data with noise*"**.
5. Under **Storing & Visualizing Data**, run the first cell to visualize the data.
   ![image](https://github.com/sidneyshafer/zumi-project/assets/66838571/e6a504c6-c6d2-437d-b18c-70ca1a290e6c)

### Data Collection
This project can be run two different ways to collect data points for classifying objects:
1. Collect data points *without* adding noise.
2. Collect data points and augment the data (add noise).
