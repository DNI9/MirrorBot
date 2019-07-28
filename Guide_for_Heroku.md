
Run the following: 

* `sudo snap install --classic heroku`

* `heroku login`
* `heroku create appname`
* `nano Aptfile` & paste ` aria2 linux `
* change download location to `/app/downloads`  in src/.constants.js
* `nano Procfile` & paste `worker: npm install -g typescript && npm install && tsc && ./aria.sh && npm start`
* `git init`
* `heroku git:remote -a appname`
* `git add .`
* `git commit -am "MirrorBot incoming, kek"`
* `git push heroku master`
* `heroku buildpacks:add --index 1 heroku-community/apt`
* `heroku ps:scale worker=1`

> if needed deploy again

To see logs:
* `heroku logs --tail -a appname`


> Thanks [@PainKiller3](https://github.com/PainKiller3/aria-telegram-mirror-bot) & Bhupy.















