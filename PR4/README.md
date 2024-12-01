# lab1
![image](https://github.com/user-attachments/assets/35e083d1-1d1d-47a3-99d6-b9eb7af3a9b3)
![image](https://github.com/user-attachments/assets/37addd40-cd8f-4fa1-8140-e04493bcec15)
![image](https://github.com/user-attachments/assets/36b2e5a2-b1e4-46d6-ba77-c7b69f8bc24a)
### Первая запись - 104.248.234.238
![image](https://github.com/user-attachments/assets/ae7b56df-238b-4e49-a805-e41337d05ce1)
### Вторая запись - array506.prod.do.dsp.mp.microsoft.com
![image](https://github.com/user-attachments/assets/c10b79dc-2491-42fb-a5cc-f138f600a3b0)
### Третья запись - tile-service.weather.microsoft.com
![image](https://github.com/user-attachments/assets/804e229e-3639-43f0-ba48-00f725fb14f1)
### Четвертая запись - array509.prod.do.dsp.mp.microsoft.com
![image](https://github.com/user-attachments/assets/47aae19e-6d10-4f82-90bd-b44468a70f50)
### Пятая и шестая записи - ctldl.windowsupdate.com и array503.prod.do.dsp.mp.microsoft.com
![image](https://github.com/user-attachments/assets/76d48244-3e8b-46fd-a94f-3c52005b686e)
### Вывод
Первая запись выглядит подозрительной, остальные являются службами/сервисами Windows и не представляют угрозы.
### Внесем последние 5 записей в safelist
![image](https://github.com/user-attachments/assets/375947f9-75bc-4f20-a5af-bd9fe37ea866)
![image](https://github.com/user-attachments/assets/7da54cc8-fc75-48f3-b482-c24dd20cd5ac)
### Длительные подключения
![image](https://github.com/user-attachments/assets/cfb70364-aa85-436a-ad4e-f672372c8e91)
![image](https://github.com/user-attachments/assets/7d1f4dbd-42ff-4f1b-af83-e18e9370a625)
![image](https://github.com/user-attachments/assets/462224cf-a64f-4339-92c0-140cc5f10c93)
![image](https://github.com/user-attachments/assets/fc735fa4-474d-4ecc-8149-04b3f2f0a366)
![image](https://github.com/user-attachments/assets/8b82106f-2144-46b5-acde-289cf6721e3e)
![image](https://github.com/user-attachments/assets/415abda6-8863-4014-8b92-dc6f225b59a3)
![image](https://github.com/user-attachments/assets/db418ee7-bba0-4ece-9d1d-fd2d9f69e1ba)
### Вывод
Соединения с кодом 104.248.234.238 наиболее вероятно нелигитмные, так как:
1. Нет FQDN запросов
2. Наибольшее количество соединений (3011) за наименьший срок
3. Изменена строка агента пользователя
4. Нет поля "host" в HTTP-заголовке
5. Длинная запутанная строка URI
6. Поиск в Google "rmvk30g" возвращает "Fiesta EK".

Все остальные записи могут быть занесены в safelist
# lab2
![image](https://github.com/user-attachments/assets/5d054155-64d8-4f2e-a01b-79c9001b59b2)
![image](https://github.com/user-attachments/assets/2fb0779f-a794-4c0d-b914-0efd00c69212)
![image](https://github.com/user-attachments/assets/5c3e8a32-4ad2-463e-9852-39a72f6c945b)
### Вывод
1. Потенциальное C2 через DNS
2. Необходима дополнительная проверка IP 
3. Возможно dnscat2
# lab3
![image](https://github.com/user-attachments/assets/63e1122c-9dd0-432f-9464-b7a38177d8d7)
![image](https://github.com/user-attachments/assets/78e7682e-95b6-46b6-a659-44c01cb4910a)
Недопустимое имя домена Skype
![image](https://github.com/user-attachments/assets/6c61a18b-af37-423f-bdcf-7366b733a58c)
Гистограммы показывают сигнатуру beacon
![image](https://github.com/user-attachments/assets/2bfb58b3-1b1b-4c7f-9844-caeb45111d49)
![image](https://github.com/user-attachments/assets/6be8b47b-236e-4146-8b88-faf9356c4566)
VirusTotal показывает плохие результаты
![image](https://github.com/user-attachments/assets/22cb7bbd-f287-46a8-b0c0-fa309241e90a)
В долгих подключениях отображаются не внесенные в безопасный список подключения
![image](https://github.com/user-attachments/assets/79122327-61e0-4b8b-a13e-89aa7f426087)
### Вывод
1. Очевидный HTTP-beacon: плоские гистограммы, пользовательский агент и FDQN выглядят ненастоящими
2. Достаточно данных для реагирования на инцидент
