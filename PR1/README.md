### Практическое задание №1. Сбор логов
1. Создать 2 виртуальные машины на базе ОС Debian 12
   ![image](https://github.com/slavastrybak/TOIB/assets/70744558/3edec274-3fea-4eee-919e-1906556563b3)
2. Обеспечить между ними сетевой обмен
   ![image](https://github.com/slavastrybak/TOIB/assets/70744558/5c00326a-f85f-478a-b4ed-d4475f09254c)
3. Включить на 1й из ВМ передачу логов по протоколу rsyslog на 2ю ВМ
   
   **Установка и настройка rsyslog**
   ![image](https://github.com/slavastrybak/TOIB/assets/70744558/9b6d4f97-ce83-42ef-8a88-355e57efda59)
   ![image](https://github.com/slavastrybak/TOIB/assets/70744558/7a3ea3dd-0e5b-4980-9e10-9ccf1c4fd4ad)
   ![image](https://github.com/slavastrybak/TOIB/assets/70744558/4430f5c2-5124-4ff8-96c8-7fed6f354d16)
   
   **Установка правил на сервер**
   ![image](https://github.com/slavastrybak/TOIB/assets/70744558/84eb36fd-2f8d-4d87-a1a6-8e7a42829670)

   **Установка правил на клиент**
   ![image](https://github.com/slavastrybak/TOIB/assets/70744558/e7072668-8d80-480d-a52f-d8e1f1b5279f)

   **Проверка**
   ![image](https://github.com/slavastrybak/TOIB/assets/70744558/078c64d8-b5bf-4d81-9135-4cf5c4d362e8)

   **Проверка получения логов на сервере**
   ![image](https://github.com/slavastrybak/TOIB/assets/70744558/e8d2042e-ad84-4daa-9534-704740ecd1e3)

4. Установить и настроить получение логов на сервер с использованием Loki
   
 **Установка и редактирование compose-файла на сервере**
 ![image](https://github.com/slavastrybak/TOIB/assets/70744558/c0684f52-fb5d-4213-86a6-29bb4f1fe9f4)
 ![image](https://github.com/slavastrybak/TOIB/assets/70744558/51f265f3-2a5e-4c26-a52f-4a73edb569b9)
   
 **Запуск Loki**
 ![image](https://github.com/slavastrybak/TOIB/assets/70744558/4d9c572e-eda8-4082-afee-57128b17fca5)

 **Редактирование promtail на клиенте**
 ![image](https://github.com/slavastrybak/TOIB/assets/70744558/ca09584e-7450-4d01-982f-e3c75f5f3c1f)

 **Compose-файл для promtail**
 ![image](https://github.com/slavastrybak/TOIB/assets/70744558/28ae2a11-e39c-4869-8368-b711bd6b3f39)

 **Запуск promtail на клиенте**
 ![image](https://github.com/slavastrybak/TOIB/assets/70744558/e1522f97-0383-4bd8-a6de-417257b35464)

 **Просмотр логов клиента в Grafana**
 ![image](https://github.com/slavastrybak/TOIB/assets/70744558/47f4db78-80ec-4e29-ba55-a2f0ded90cbc)
 


   
   





