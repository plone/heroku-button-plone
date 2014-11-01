Free Plone site on Heroku
=========================

It takes just a few short minutes to deploy your very own Plone site in the
cloud and run it for free. Just click this button and follow the instructions.

[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy?template=https://github.com/plone/heroku-button-plone)

After the site is up you can read [how to get the most of Plone on Heroku](https://github.com/plone/heroku-buildpack-plone#sparkles-bonus-karma-points-sparkles).


Run your Plone site on your local machine
-----------------------------------------

You can also clone this code from Heroku into your local machine, and run Plone locally, for example, to test something out (this assumes you have Python 2.7 and the Heroku Toolbelt installed on your machine):

    $ heroku login
    $ heroku git:clone -a <YOUR_APP_NAME>
    $ cd <YOU_APP_NAME>

    $ curl -OL "http://downloads.buildout.org/1/bootstrap.py"
    $ python2.7 bootstrap.py
    $ bin/buildout
    $ bin/instance fg

Now open your browser and point it to ``http://localhost:8080``. Login with
`admin:admin`.
