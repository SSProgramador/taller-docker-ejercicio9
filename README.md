# taller-docker-ejercicio9
Bot de telegram

# Crear el namespace
kubectl create namespace telegrambot

# Aplicar el configmap
kubectl apply -f configmap-env.yaml -n telegrambot

# Aplicar el deployment
kubectl apply -f deployment.yaml -n telegrambot

# Aplicar el servicio
kubectl apply -f service.yaml -n telegrambot

# Verificar que todo funciona
kubectl get services -n telegrambot