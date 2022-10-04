# machine_learning-2022-
Gahchon Univ/machine_learning(2022)
function of phw#1 large function
# file 1: AutoML.ipynb
```markdown
function AutoML
```
# file 2: Applying_Example.ipynb
```markdown
appliying AutoML function to dataset(preprocessing + applying to AutoML function + analysis result)
```
* used_data : california housing prices dataset(housing.csv)
dataset link : <https://www.kaggle.com/camnugent/california-housing-prices>

# function: Auto ML
```markdown
* function AutoML : return dataframe to store all parameter’s and measuring result of each model
* input : scaler_list, encoder_list, model_list, hyperparmeter_df, dataset_no_target, dataset_target, categorical_attr_list, measure_df
* output : function_result_df
```

## scaling

|standard|minmax|maxabs|robust|norm|
|------|---|---|---|---|

## encoder

|label|onehot|ordinal|
|------|---|---|

## model

|model_name|K-means|EM|CLARANS|DBSCAN|AffinityPropagation|
|----|------|---|---|---|---|
|parameter|n_clusters, algorithm|n_component, covariance_type|number_clusters, maxneighbor|eps, min_samples|preference, max_iter|

## measure
|model_name|K-means|EM,CLARANS,DBSCAN,AffinityPropagation|
|----|------|---|
|measure_tool|knee-method, purity, silhouette_score|purity, silhouette_score|

### func1:	cal_cluster_mean
```markdown
* function cal_cluster_mean : calculater all cluster’s attirbute’s mean using labeled data
* input : dt_n_t, answer_df, k (*dt_n_t = dataset_no_target)
* output : cluster_mean_list
```

### func2:	pca_visualize
```markdown
* function pca_visualize : make dataset to 2D using pca and visualize them.
* input : dataset_no_target, y_pred,k, model_name,params
* output : nothing (just visualize pca plot)
```

### func3:	make_result_list
```markdown
* function make_result_list : append all parameters and make result to return
* input : scaling_type, encoding_type, model_name, parameters, knee, score1, score2 , dist
* output : result_list
```
