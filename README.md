# php-app

## Helm chart для деплоя php приложений

## Пример использования: 

helm upgrade -i example oci://harbor.example.ru/apps/php-app -n default --set replicaCount=2 --set persistance.path=example --set 'hosts[0].name=example.example.ru,hosts[0].root=/,hosts[0].tls.enable=false'

Чарт заливается в harbor, все необходимые настройки в values.yaml