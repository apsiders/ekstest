# ekstest
Prueba de creación cluster de kubernetes con aws eks. 

## Previo
Antes de ejecutar cambie las subnet por las suyas.

## Para Crear
Para crear el cluster ejecute lo siguiente:
```
eksctl create cluster -f eks-test.yaml --auto-kubeconfig
```

## Para descargar el archivo kubeconfig
Ejecute lo siguiente para obtener el kubeconfig.
```
aws eks --region us-east-1 update-kubeconfig --name eks-test
```

## Para Eliminar:
Para eliminar el cluster ejecute lo siguiente:
```
eksctl delete cluster --name=eks-test
```