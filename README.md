This is a basic Sinatra application. 

Deploy this application on Heroku to complete 
lesson challenge #1. 

View the complete lesson on deploying this app: 
http://blog.heroku.com/archives/2009/3/5/32_deploy_merb_sinatra_or_any_rack_app_to_heroku/

-----------------------------

**** Help with Tutorial ****

As it turns out, the tutorial on Heroku neglects to mention 
that in order to call `run Sinatra::Application` you need 
to have the sinatra gem installed in your repository. To do 
that with bundler, create a gemfile.

    touch Gemfile
    vim $!

Add the rubygems gem repository and then the sinatra gem. 

    1: source :rubygems
    2:
    3: gem 'sinatra'   

Then push this to Heroku and it should download and install 
sinatra for you. After that the app should run. 

