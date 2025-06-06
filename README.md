# Домашнее задание "Система сбора логов Elastic Stack"   

---

### Задание 1 

Вам необходимо поднять в докере и связать между собой:

- elasticsearch (hot и warm ноды);
- logstash;
- kibana;
- filebeat.
Logstash следует сконфигурировать для приёма по tcp json-сообщений.

Filebeat следует сконфигурировать для отправки логов docker вашей системы в logstash.
В директории [help](https://github.com/netology-code/mnt-homeworks/tree/MNT-video/10-monitoring-04-elk/help) находится манифест docker-compose и конфигурации filebeat/logstash для быстрого выполнения этого задания.
Результатом выполнения задания должны быть:

- скриншот docker ps через 5 минут после старта всех контейнеров (их должно быть 5);
- скриншот интерфейса kibana;
- docker-compose манифест (если вы не использовали директорию help);
- ваши yml-конфигурации для стека (если вы не использовали директорию help).


![image.jpg](https://github.com/temagraf/Elastic-Stack/blob/main/1.png)

- Cкриншот docker ps через 5 минут после старта всех контейнеров (их должно быть 5):

![image.j](https://github.com/temagraf/Elastic-Stack/blob/main/2.png)

- скриншот интерфейса kibana:
  
![image.jpg](https://github.com/temagraf/Elastic-Stack/blob/main/3.png)



---

### Задание 2

Перейдите в меню создания index-patterns в kibana и создайте несколько index-patterns из имеющихся.  

Перейдите в меню просмотра логов в kibana (Discover) и самостоятельно изучите, как отображаются логи и как производить поиск по логам.  

В манифесте директории help также приведенно dummy-приложение, которое генерирует рандомные события в stdout-контейнера. Эти логи должны порождать индекс logstash-* в elasticsearch. Если этого индекса нет — воспользуйтесь советами и источниками из раздела «Дополнительные ссылки» этого задания.  
 

- Перейдите в меню создания index-patterns в kibana и создайте несколько index-patterns из имеющихся:

  
![image.jpg](https://github.com/temagraf/Elastic-Stack/blob/main/2-1.png)


![image.jpg](https://github.com/temagraf/Elastic-Stack/blob/main/2-2.png)


- Перейдите в меню просмотра логов в kibana (Discover) и самостоятельно изучите, как отображаются логи и как производить поиск по логам:

![image.jpg](https://github.com/temagraf/Elastic-Stack/blob/main/2-3.png)


![image.jpg](https://github.com/temagraf/Elastic-Stack/blob/main/2-4.png)


![image.jpg](https://github.com/temagraf/Elastic-Stack/blob/main/2-5.png)
