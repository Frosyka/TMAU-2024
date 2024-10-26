<p align="center">Министерство образования Республики Беларусь</p>
<p align="center">Учреждение образования</p>
<p align="center">“Брестский Государственный технический университет”</p>
<p align="center">Кафедра ИИТ</p>
<br><br><br><br><br><br>
<p align="center"><strong>Лабораторная работа №3</strong></p>
<p align="center"><strong>По дисциплине</strong> “Теория и методы автоматического управления”</p>
<p align="center"><strong>Тема:</strong> “Работа с контроллером AXC F 2152”</p>
<br><br><br><br><br><br>
<p align="right"><strong>Выполнил</strong>:</p>
<p align="right">Студент 3 курса</p>
<p align="right">Группы АС-63</p>
<p align="right">Карпеш Н.П.</p>
<p align="right"><strong>Проверил:</strong></p>
<p align="right">Ситковец Я.С.</p>
<br><br><br><br><br>
<p align="center"><strong>Брест 2024</strong></p>

---
<p> <strong>Цель:</strong> разработать тестовый проект "Hello PLCnext from AS0xxyy!", собрать его и продемонстрировать его работоспособность на тестовом контроллере.</p>

<p> <strong>Решение:</strong> </p>
<p>В соответствии с заданием, начинаем с клонирования репозитория.</p>
<p>Для сборки файла <em>hello_PLCnext</em> используем следующие команды:</p>


 ``` bash
cmake --preset=build-windows-AXCF2152-2021.0.3.35554 .
```


 ``` bash
cmake --build --preset=build-windows-AXCF2152-2021.0.3.35554 --target all
```



 ``` bash
cmake --build --preset=build-windows-AXCF2152-2021.0.3.35554 --target install
```

<p>Подключаем контроллер и настраиваем сетевые параметры для обеспечения взаимодействия с ним.</p>

![](images/connect.png)  

<p>Необходимо проверить, что подключение к контроллеру установлено успешно.</p>

![](images/network_configuration.png)  

<p>Запускаем программу <em>PuTTY Configuration</em> и осуществляем подключение к контроллеру.</p>

![](images/PuTTY_connect.png) 

<p>Вводим логин и пароль для доступа к контроллеру.</p>

![](images/PuTTY_login_password.png) 

<p>Запускаем <em>WinCP</em>, после чего подключаемся к контроллеру.</p>

![](images/WinCP_connect.png) 

<p>Переносим собранный проект в корневую директорию контроллера и изменяем его разрешения для возможности запуска.</p>

![](images/hello_PLCnext_settings.png) 

<p>Запускаем проект и получаем результат.</p>

![](images/result.png) 

<p> <strong>Вывод:</strong> В ходе данной лабораторной работы был разработан тестовый проект "Hello PLCnext from AS0xxyy!", что позволило получить полезные знания для работы с контроллером <em>AXC F 2152</em></p>