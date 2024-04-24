# ParameterOptimization
## Methodology:
1. Data Loading and Preprocessing: The dataset "Dry_Bean_Dataset.csv" is loaded into a Pandas DataFrame. Features (X) and labels (Y) are separated, and Standard Scaling is applied to normalize the features.
2. Data Splitting: The data is split into training and testing sets using a 70-30 split for 10 different random states. This is to ensure the robustness of the model by testing it on different data splits.
3. Model Selection: Support Vector Machine (SVM) with different kernels (linear, poly, rbf, sigmoid) is used as the base model.
4. Hyperparameter Optimization: For each random split, a random search is conducted for the hyperparameters C and gamma for each kernel. The C and gamma values are randomly sampled from a uniform distribution 
   between 0 and 10. The model's accuracy is evaluated using the accuracy_score metric.
5. Convergence Analysis: The convergence of the accuracy scores over iterations is plotted to visualize the model's performance improvement over iterations.
## Result Table:
The result table contains the following columns:

1. Sample: The identifier for each random split.
2.BestAccuracy: The best accuracy achieved for each split.
3.BestC: The best C value for each split.
4.BestGamma: The best gamma value for each split.
5.BestKernel: The best kernel for each split.

![image](https://github.com/rhy004/ParameterOptimization/assets/91721588/66b8210c-9611-4d64-b3db-56715e33e34a)

## Result Graph:
The result graph shows the convergence of accuracy scores over iterations for each random split. Each line represents the convergence of accuracy scores for a specific random split, illustrating how the accuracy score changes with each iteration.

![image](https://github.com/rhy004/ParameterOptimization/assets/91721588/a9c82112-f458-44d9-b462-d9b8488d7544)
