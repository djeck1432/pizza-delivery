# Bot shop
 This is ```Telegram Shop```, where there is an opportunity to:
 • choose an item,
 • choose the amount,
 • go back and navigate through menu items,
 • add the item and delete it,
 • see what is in the basket,
 • leave an email for a feedback. You can try the functional <a href='https://t.me/DevmanLesson3_bot'>here</a>

## Instruction for running code on the server

### Registration and installation of Heroku

Sign up on this  <a href='https://signup.heroku.com/dc'>site</a>.
<br>
To work through the terminal install ```CLI``` for ```Heroku```, to do this you should open ``bash`` on your computer and write in there next commands: 
<br>
For Linux  ```Linux``` -<br>
```sudo snap install heroku --classic```
<br>
For ```MacOs``` - <br>
```brew install heroku/brew/heroku```
<br>
Staying in the terminal, log into your account on ```Heroku``` with ```bash```:
<br>
```heroku login```
<br>
### Загрузка кода на сервер Heroku

Загрузите с ```github``` ваш репозиторий на компьютер: 
<br>
```git clone https://github.com/djeck1432/telegram_shop.git```
<br>
Откройте папку:
<br>
```cd telegram_shop ```
<br>
Создайте приложения в ```Heroku``` :
<br>
```heroku create```
<br>
Загрузите ваш репозиторий на сервер ```Heroku```:
<br>
```git push heroku master```
<br>

### Настройка окружения и запуск сервера

Перейдите по <a href='https://dashboard.heroku.com/apps'>ссылке</a>, выберите свое приложение и откройте его.
<br>
В меню навигации, перейдите на вкладку ```Settings```.
<br>
В разделе ```Config vars```, передайте ваши переменные окружения.
<br>
В терминале, выполните следующую команду для запуска кода на сервере:<br>
```heroku ps:scale bot=1```
<br>
Поздравляю, теперь ваш ```Bot``` работает постоянно, вне зависимости, включен ваш компьютер или нет.
<a name='env'></a>

## Переменные окружения 
Параметры CMS ```Moltin```:
<br>
```STORE_ID``` - ```id``` магазина;
<br>
```CLIENT_ID```- ```id``` клиента;
<br>
```CLIENT_TOKEN```- токен 
<br>
```TELEGRAM_ACCESS_TOKEN```- ```Telegram``` токен;
<br>

Параметры базы данных ```Redis``` :
<br>
```REDIS_PASSWORD ```-  пароль;
<br>
```REDIS_PORT```- порт;
<br>
```REDIS_HOST```- хост;
