<p>This was hosted on heroku with posgresql. the link for the site is http://sleepy-dawn-12657.herokuapp.com/</p></br>
<p>built using the udemy course by edwin diaz https://www.udemy.com/course/laravel-deployment/</p></br>
<p>The following steps for heroku deployment of laravel found in the folloing link: https://devcenter.heroku.com/articles/getting-started-with-laravel</p></br>

<p>first create a larave project and add it to git then use the following commands:</p></br>
<p>login to heroku using : heroku login</p></br>
<p>create app: heroku create</p></br>
<p>link with heroku with local: heroku buildpacks:set heroku/php</p></br>
<p>set the app key in heroku with local app key using cmd: heroku config:set APP_KEY=base64:qcpfNQJNYKPjTjM8IxOZpevukW4Sbs4F9b2aClIH95I=</p></br>
<p>create heroku proc file: echo "web: vendor/bin/heroku-php-apache2 public/" > Procfile</p></br>
<p>git add .</p></br>
<p>git commit -m "procfile add"</p></br>
<p>git push heroku master</p></br>
<p>heroku open</p></br>
<p>to run command in heroku online: heroku run php artisan migrate to connect to database in heroku go to resources add postgres(free) and get the db credentials and use them in heroku app env file by going to settings > add config variables</p></br>
