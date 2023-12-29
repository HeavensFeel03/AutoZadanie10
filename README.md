# План автоматизации тестирования перехода к форме записи и заполнения этой формы.
### 1. Перечень автоматизируемых сценариев.
##### Тестирование возможности записаться на обучение профессии «Тестировщик ПО».
Через «Каталог курсов»
*	На главной странице сайта https://netology.ru/ нажать кнопку «Каталог Курсов».
*	В появившемся блоке выбрать раздел «Программирование».
*	В появившейся странице в окне поиска ввести и выбрать «Тестировщик ПО»
*	Перейти к форме записи на курс нажав кнопку «Записаться».
*	Ввести данные в поля и нажать кнопку «Записаться»
  
Через «Направление обучения»
* На главной странице сайта https://netology.ru/ перейти к блоку «Направления обучения».
*	В блоке выбрать раздел «Программирование».
*	В появившейся странице в окне поиска ввести и выбрать «Тестировщик ПО»
*	Перейти к форме записи на курс нажав кнопку «Записаться».
*	Ввести данные в поля и нажать кнопку «Записаться»
  
Через «Подвал» сайта
*	На главной странице сайта https://netology.ru/ спуститься в конец страницы сайта.
*	В разделе «Обучение» выбрать «Каталог курсов»
*	В появившейся странице в окне поиска ввести и выбрать «Тестировщик ПО»
*	Перейти к форме записи на курс нажав кнопку «Записаться».
*	Ввести данные в поля и нажать кнопку «Записаться»
##### Валидация полей в форме записи на обучение профессии «Тестировщик ПО».
Позитивный результат в поле «Имя»
*	Ввести имя на кириллице. Например: "Александр" 
*	Ввести имя на латинице. Например: "Alex"
*	Ввести двойное имя через пробел. Например: "Александр Василий"
*	Ввести двойное имя через дефис. Например: "Алесандр-Василий"
*	Ввести имя с буквой ё. Например: "Лёша"
*	Ввести текст, длиной в 40 символов. 

*Ожидаемый результат:* Поле "Имя" заполнено
  
Негативный результат в поле «Имя»
*	Ввести текст, длиной в 41 символов.*Ожидаемый результат:* Вывод сообщения: "Слишком много символов"
*	Оставить пустым поле «Имя».*Ожидаемый результат:* Вывод сообщения: "Поле должно быть заполнено"
*	Ввести спецсимволы. Например: "$" *Ожидаемый результат:* Вывод сообщения: "Не допускаются спецсимволы"
*	Ввести цифры.Например: "234234" *Ожидаемый результат:* Вывод сообщения: "Не допускаются цифры"
*	Ввести иероглифы. Например: "的" *Ожидаемый результат:* Вывод сообщения: "Не допускаются иероглифы"
  
Позитивный результат в поле «Телефон».
*	Ввести номер телефона из 11 цифр. Например: "89085938210".

*Ожидаемый результат:* Поле "Телефон" заполнено.
  
Негативный результат в поле «Телефон».
* Оставить пустым поле «Телефон». *Ожидаемый результат:* Вывод сообщения: "Поле должно быть заполнено"
*	Ввести 10 цифр. *Ожидаемый результат:* Вывод сообщения: "В поле не должно быть меньше символов чем 11"
*	Ввести кириллицу. Например: "ваыав" *Ожидаемый результат:* Вывод сообщения: "Не допускается кириллица"
*	Ввести латиницу. Например: "fsdfsd" *Ожидаемый результат:* Вывод сообщения: "Не допускается латиница"
*	Ввести спецсимволы. Например: "$" *Ожидаемый результат:* Вывод сообщения: "Не допускаются спецсимволы"

#####	Оформление заявки на форме записи.
* Сценарий 1. Поля "Имя" и "Телефон" заполнены валидными данными.

Пример: В поле "Имя" ввести "Александр". В поле "Телефон" ввести "89085938210".

*Ожидаемый результат:* Вывод сообщения "Заявка принята".

* Сценарий 2. Поля "Имя" и "Телефон" остаются пустыми.

*Ожидаемый результат:* Вывод сообщения "Поля должны быть заполнены".

* Сценарий 3. Поле "Имя" заполнено валидными данными. Поле "Телефон" заполнено невалидными данными.
  
Пример: В поле "Имя" ввести "Александр". В поле "Телефон" ввести "sdada".

*Ожидаемый результат:* Вывод сообщения: "Не допускается латиница в поле телефон".

* Сценарий 4. Поле "Имя" заполнено невалидными данными. Поле "Телефон" заполнено валидными данными.

Пример: В поле "Имя" ввести "$$$$". В поле "Телефон" ввести "89085938210".

*Ожидаемый результат:* Вывод сообщения: "Не допускаются спесимволы в поле имя".

### 2.Перечень используемых инструментов с обоснованием выбора.
*	Google Chrome - браузер, для исследования тестируемой страницы
* IntelliJ IDEA - среда разработки программного обеспечения для написания кода.
* Java - язык программирования для написания автотестов.
* Gradle — система управления проектами. Инструмент автоматизации сборки и управления зависимостями, которые сами выкачивают нужные вам библиотеки и их зависимости.
* JUnit - среда тестирования для приложений Java
* Selenide - фреймворк для автоматизированного тестирования веб-приложений на основе Selenium WebDriver .
*	Allure Framework - фреймворк, который служит для получения отчетов о прохождении авто-тестов.
*	Lombok - основанная на аннотациях библиотека Java, позволяющая сократить шаблонный код
* Faker - библиотека, для генерации тестовых данных.

### 3. Перечень необходимых разрешений, данных и доступов.
Нужно получить разрешение на тестирование и автоматизацию. Также нужно получить тестовый вариант сайта.
### 4. Перечень и описание возможных рисков при автоматизации.
* Утечка личных данных пользователей.
* Автоматизация требует постоянной поддержки.
* Дополнительные финансовые затраты на инфраструктуру.
### 5. Перечень необходимых специалистов для автоматизации.
Тестировщик, с навыками автоматизации тестирования
### 6. Интервальная оценка с учётом рисков в часах.
30 часов






