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
### Download code on Heroku

Download from ```github``` your repository to computer:
<br>
```git clone https://github.com/djeck1432/pizza-delivery.git```
<br>
Open the folder:
<br>
```cd pizza-delivery ```
<br>
Create a new app on ```Heroku``` :
<br>
```heroku create```
<br>
Download your repository on the server ```Heroku```:
<br>
```git push heroku master```
<br>

### Setting up the environment and starting the server

Go to the <a href='https://dashboard.heroku.com/apps'>link</a>, choose your app and open it.
<br>
In the navigation menu, go to the tab ```Settings```.
<br>
In chapter```Config vars```, pass your environment variables.
<br>
In the terminal, do the next command for start code on the server:<br>
```heroku ps:scale bot=1```
<br>
Congratulations, now your `` Bot`` is constantly working.
<a name='env'></a>


## Environment variables 
 Parametrs CMS ```Moltin```:
<br>
```STORE_ID``` - ```id``` shop;
<br>
```CLIENT_ID```- ```id``` client;
<br>
```CLIENT_TOKEN```- token 
<br>
```TELEGRAM_ACCESS_TOKEN```- ```Telegram``` token;
<br>

Database options ```Redis``` :
<br>
```REDIS_PASSWORD ```-  password;
<br>
```REDIS_PORT```- port;
<br>
```REDIS_HOST```- host;
