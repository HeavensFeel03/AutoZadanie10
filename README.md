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
*	Ввести имя на кириллице
*	Ввести имя на латинице
*	Ввести двойное имя через пробел
*	Ввести двойное имя через дефис
*	Ввести имя с буквой ё
*	Ввести текст, длиной в 40 символов
  
Негативный результат в поле «Имя»
*	Ввести текст, длиной в 41 символов
*	Оставить пустым поле «Имя»
*	Ввести спецсимволы
*	Ввести цифры
*	Ввести иероглифы
  
Позитивный результат в поле «Телефон»
*	Ввести номер телефона из 11 цифр
  
Негативный результат в поле «Телефон»
* Оставить пустым поле «Телефон»
*	Ввести 10 цифр
*	Ввести кириллицу
*	Ввести латиницу
*	Ввести спецсимволы

#####	Оформление заявки на форме записи
*	Ввести в поля «Имя» и «Телефон» валидные данные
*	Ввести в поля «Имя» и «Телефон» невалидные данные

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






