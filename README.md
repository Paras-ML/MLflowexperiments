##MLFLOW Experiments

import dagshub
dagshub.init(repo_owner='sharmaparas23', repo_name='MLflowexperiments', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)