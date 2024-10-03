# MLFlow-Basics

## For Dagshub:
import dagshub
dagshub.init(repo_owner='Muntasir-Ayan', repo_name='MLFlow-Basics', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)

  ''' bash
  export MLFLOW_TRACKING_URI=https://dagshub.com/Muntasir-Ayan/MLFlow-Basics.mlflow
  export MLFLOW_TRACKING_USERNAME=Muntasir-Ayan

  '''