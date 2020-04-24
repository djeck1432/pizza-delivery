# Pizza delivery Bot
 There are ```Telegram Bot``` and ```Facebook Bot``` , where there is an opportunity to:
 <ol> 
 <li>choose an item,</li>
 <li>choose the amount,</li>
 <li>go back and navigate through menu items,</li>
 <li>add the item and delete it,</li>
 <li>see what is in the basket,</li>
 <li>leave an email for a feedback.</li>
</ol>
 You can try the functional <a href='https://t.me/DevmanLesson3_bot'>here</a> .

## Instruction for running code on the server

### Registration and installation of Heroku

Sign up on this <a href='https://signup.heroku.com/dc'>site</a>

To work through the terminal install `CLI` for `Heroku`, to do this you should open `bash` on your computer and write in there next commands: 

For Linux  `Linux` -
```
sudo snap install heroku --classic
```

For `MacOs` -
```
brew install heroku/brew/heroku
```

Staying in the terminal, log into your account on `Heroku` with `bash`:
```
heroku login
```
### Download code on Heroku

Download from `github` your repository to computer:
```
git clone https://github.com/djeck1432/pizza-delivery.git
```
Open the folder:
```
cd pizza-delivery
```
Create a new app on `Heroku` :
```
heroku create
```
Download your repository on the server `Heroku`:
```
git push heroku master
```

### Setting up the environment and starting the server

Go to the <a href='https://dashboard.heroku.com/apps'>link</a>, choose your app and open it.

In the navigation menu, go to the tab `Settings`.

In chapter `Config vars`, pass your environment variables.

In the terminal, do the next command for start code on the server:
```
heroku ps:scale bot=1
```

Congratulations, now your `Bot` is constantly working.
<a name='env'></a>


## Environment variables 
 Parametrs CMS `Moltin`:
 
`STORE_ID` - `id` shop;

`CLIENT_ID`- `id` client;

`CLIENT_TOKEN`- token 

`TELEGRAM_ACCESS_TOKEN`- `Telegram` token;


Database options `Redis` :

`REDIS_PASSWORD`-  password;

`REDIS_PORT`- port;

`REDIS_HOST`- host;
