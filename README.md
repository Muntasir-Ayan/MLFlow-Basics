# MLFlow-Basics

## For Dagshub:
import dagshub
dagshub.init(repo_owner='Muntasir-Ayan', repo_name='MLFlow-Basics', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)

  ''' bash
  set MLFLOW_TRACKING_URI=https://dagshub.com/Muntasir-Ayan/MLFlow-Basics.mlflow
  set MLFLOW_TRACKING_USERNAME=Muntasir-Ayan
  set MLFLOW_TRACKING_PASSWORD=42d57fdaae1f2c0e83d19ee1f519731e73a36964

  '''