## MLOps - experiments with mlflow

import dagshub
dagshub.init(repo_owner='susamay.sk', repo_name='mlflow-dagshub-bentoml-pipeline', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)