# artsiomrudenia_platform
# Выполнено ДЗ №1

 - [x] Основное ДЗ
 - [ ] Задание со *

## В процессе сделано:
 - Из Dockerfile собран образ контейнера, в который маунтится homework.html
 - Все pod в своем yaml-файле имеют restartPolicy: Always.
Различные pod управляются различными контроллерами (Deployment-контроллер, ReplicaSet-контроллер и т.д.).
Т.к. контроллер запрашивает у API состояние объектов, которые он контролирует, то после удаления он получает статус пода из API и триггерит Scheduler, который дает приказ kubelet развернуть под.

## Как запустить проект:
 - http://localhost:8000/homework.html

## Как проверить работоспособность:
 - Запустить curl http://localhost:8000/homework.html 

## PR checklist:
 - [x] Выставлен label с номером домашнего задания

# Выполнено ДЗ №2

 - [x] Основное ДЗ
 - [x] Задание со *

## В процессе сделано:
 - Создали replicaset и deployments для сервисов frontend и paymentservice. Для frontend deployment добавлена readiness probe.
 - ReplicaSet не обновляет версии запущенных под, т.к. следит только за их количеством.
 - Для paymentservice созданы 2 доп. варианта развертывания: blue-green и reverse
 - 

## PR checklist:
 - [x] Выставлен label с номером домашнего задания