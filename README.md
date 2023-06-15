# Домашнее задание к занятию "11.2 «ELK»" - Соловьёв Андрей SYS-18

---

## Задание 1. Elasticsearch

Установите и запустите Elasticsearch, после чего поменяйте параметр cluster_name на случайный.

- Elasticsearch установлен и запущен:

![elasticsearch_started](https://github.com/Andrewsolo1969/11-3-hw/blob/main/img/elasticsearch_started.png)

Приведите скриншот команды 'curl -X GET 'localhost:9200/_cluster/health?pretty', сделанной на сервере с установленным Elasticsearch. Где будет виден нестандартный cluster_name.

- cluster_name содержится в файле /etc/elasticsearch/elasticsearch.yml, соответственно меняем этот параметр:

nano /etc/elasticsearch/elasticsearch.yml

![elasticsearch_node_name](https://github.com/Andrewsolo1969/11-3-hw/blob/main/img/elasticsearch_node_name.png)

Результат команды curl -X GET 'localhost:9200/_cluster/health?pretty

![elasticsearch_1](https://github.com/Andrewsolo1969/11-3-hw/blob/main/img/elasticsearch_1.png)

То же через браузер

![elasticsearch_2](https://github.com/Andrewsolo1969/11-3-hw/blob/main/img/elasticsearch_2.png)


## Задание 2. Kibana

Установите и запустите Kibana. - Kibana установлена и запущена:

![kibana_started](https://github.com/Andrewsolo1969/11-3-hw/blob/main/img/kibana_started.png)

Приведите скриншот интерфейса Kibana на странице http://<ip вашего сервера>:5601/app/dev_tools#/console, где будет выполнен запрос GET /_cluster/health?pretty:

![Kibana_full](https://github.com/Andrewsolo1969/11-3-hw/blob/main/img/Kibana_full.png)

![Kibana_short](https://github.com/Andrewsolo1969/11-3-hw/blob/main/img/Kibana_short.png)


## Задание 3. Logstash

Установите и запустите Logstash и Nginx. С помощью Logstash отправьте access-лог Nginx в Elasticsearch.

- Logstash установлен и запущен:

![Logstash_started](https://github.com/Andrewsolo1969/11-3-hw/blob/main/img/Logstash_started.png)

Приведите скриншот интерфейса Kibana, на котором видны логи Nginx.


## Задание 4. Filebeat

Установите и запустите Filebeat. Переключите поставку логов Nginx с Logstash на Filebeat.

- Filebeat установлен и запущен:

![filebeat_started](https://github.com/Andrewsolo1969/11-3-hw/blob/main/img/filebeat_started.png)

Приведите скриншот интерфейса Kibana, на котором видны логи Nginx, которые были отправлены через Filebeat.













 
