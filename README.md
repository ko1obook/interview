# Interview

## Описание

Создание масштабируемой системы обработки данных. Проработаны этапы от приема данных до обработки и хранения, используя надежный технический стек: Apache Airflow, Python, Apache Kafka, Apache Zookeeper, Apache Spark и Cassandra. Все контейнеризовано с помощью Docker для простоты развертывания и масштабируемости.

## Архитектура
Источник данных: API randomuser.me для генерации случайных пользовательских данных для нашего конвейера.  
Apache Airflow: Отвечает за организацию конвейера и хранение извлеченных данных в базе данных PostgreSQL.  
Apache Kafka и Zookeeper: Используются для потоковой передачи данных из PostgreSQL в обрабатывающий механизм.  
Control Center и Schema Registry: Помогают в мониторинге и управлении схемами наших потоков Kafka.  
Apache Spark: Для обработки данных с его главными и рабочими узлами.  
Cassandra: Хранение обработанных данных.  