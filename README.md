heroku
======
git clone https://github.com/boy12371/heroku.git
cd heroku
heroku create heroku -s cedar
heroku config:add BUILDPACK_URL="https://github.com/archaelus/heroku-buildpack-erlang.git" -a heroku
git push heroku master
curl http://heroku.herokuapp.com
