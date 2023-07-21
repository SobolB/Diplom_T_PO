# Дипломный проект профессии «Тестировщик»

[План автоматизации](https://github.com/SobolB/Diplom_T_PO/blob/master/docs/Plan.md)

[Отчет по итогам тестирования](https://github.com/SobolB/Diplom_T_PO/blob/master/docs/Report.md)

[Отчет по итогам автоматизации](https://github.com/SobolB/Diplom_T_PO/blob/master/docs/Summary.md)

---------------------
## Инструкция по запуску

#### 1. Склонировать репозиторий  
  <code>git clone https://github.com/SobolB/Diplom_T_PO.git</code>

#### 2.  Перейти в папку <ins>Diplom_T_PO</ins>  

#### 3. Для работы с базой данных включаем приложение Wampser64:
   
  ![image](https://github.com/SobolB/Diplom_T_PO/assets/79850869/4384ada9-5eeb-4944-a031-0b43770ae35f)
  ![image](https://github.com/SobolB/Diplom_T_PO/assets/79850869/7f758a11-b480-462f-91c6-f210732702d9)

#### 4. В файле <ins> [application.properties](https://github.com/SobolB/Diplom_T_PO/blob/master/application.properties) </ins>, меняем данные на свои:
  * Изменяем ссылку <ins>spring.datasource.url</ins> (url) на свою
  * Изменяем поле <ins>spring.datasource.username</ins> (username) на свое
  * Изменяем поле <ins>spring.datasource.password</ins> (password) на свое

  ![image](https://github.com/SobolB/Diplom_T_PO/assets/79850869/25104042-1edc-412c-94e0-82902427a574)

#### 5. Запускаем тесты:
     
  Открываем Terminal Local (1):
   
  Вводим команды:
   
  <code>cd gate-simulator</code>
    
  <code>node app.js</code>
    
  ![image](https://github.com/SobolB/Diplom_T_PO/assets/79850869/7ddd0e2d-47b4-4943-9d05-d413b6659bc0)

#### 6. Открываем Terminal Local (2):
  
  Вводим команды:
    
  <code>cd artifacts</code>
    
  <code>java -jar aqa-shop.jar</code>
    
  ![image](https://github.com/SobolB/Diplom_T_PO/assets/79850869/dff8986a-8593-4851-9208-f673ef430558)
    
#### 7.  Запуск тестов:
  
  Выделяем два теста, нажимаем правой кнопкой мыши на любой из тестов и запускаем.

  ![image](https://github.com/SobolB/Diplom_T_PO/assets/79850869/3fae4424-a230-4d34-89a0-f1b75d9a6102)
  ![image](https://github.com/SobolB/Diplom_T_PO/assets/79850869/9d30a965-45e0-48b8-b713-9eadb0bb0aa2)

#### 8. Сформируем отчет allure:
 
  Открываем Terminal Local (3):
    
  Вводим команду:
    
  <code>allure generate build/allure-results --clean</code>,
  где <code>--clean</code> используется для очистки информации и обновления ее
    
  ![image](https://github.com/SobolB/Diplom_T_PO/assets/79850869/18264642-6abb-455c-a002-689b0fa89aff)
   
#### 9. Открываем отчет в браузере:
 
  Открываем файл <ins>allure-report</ins>, находим файл <ins>index.html</ins> и открываем с помощью браузера.
  ![image](https://github.com/SobolB/Diplom_T_PO/assets/79850869/7993c5d5-f26f-4772-8f39-b83e01ab4bb0)
  ![image](https://github.com/SobolB/Diplom_T_PO/assets/79850869/35f2d2ff-1c33-46cf-a6e1-1a9ade8edce1)

