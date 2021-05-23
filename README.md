# How to run

All commands are available in commands.txt

#### Firstly download DB using helm
1. ``` helm upgrade --install postgres-helm ./postgres-helm ```
 
#### Secondly apply yaml files
2. ``` kubectl apply -f ConfigMap.yaml -f Secrets.yaml -f DjangoDeployment.yaml ```

#### Thirdly run django backend in 8000 port to check all requests
3. ``` kubectl port-forward "backend pod name" 8000:8000 ```
