# machine_learning-2022-
Gahchon Univ/machine_learning(2022)
function of phw#1 large function
# file 1: Giant Function.ipynb
```markdown
function ML + function make_result_list
```
# file 2: Applying_Example.ipynb
```markdown
appliying giant function to dataset(preprocessing + applying to giant function + analysis result)
```
* used_data : breast-cancer-wisconsin.data, breast-cancer-wisconsin.names
dataset link : <https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/>

# func1: Giant Function ML
```markdown
* function ML : do dataset scaling, make model, calculate accuracy score and return that info using dataframe form \n
* input : scaling_type, algorithm_name, dataset_no_target, dataset_target
* output : function_reusult_dataframe
```

## scaling

|none|standard|minmax|
|------|---|---|

## model

|model_name|deicision_tree(entropy)|decision_tree(gini)|logistic_regression|SVM|
|----|------|---|---|---|
|parameter|max_depth : [1,10]|max_depth : [1,10]|C_param :  [0.0001]|C_param :  [0.0001, 0.001]|

## train_test_split
|k_fold|5, 10|
|---|---|

# func2:	Make_result_list
```markdown
* function make_result_list : make one line(list) of function ML's return dataframe
* input : scaling_type, algorithm_name, k_fold_param, algorithm_param, accuracy
* output : result_list
```

