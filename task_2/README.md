Task 2

Инструкция по запуску

Создайте namespace:
kubectl apply -f namespace.yaml
Создайте deployment:
kubectl apply -f deployment.yaml
Инструкция по проверке

Проверьте, что поды запущены в namespace homework:
kubectl get pods -n homework
Убедитесь, что все поды находятся в статусе READY 1/1 и STATUS Running.
Для проверки логов одного из подов выполните:
kubectl logs <pod-name> -n homework
