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

    source :rubygems
    
    gem 'sinatra'   

Save the file and add it to the local git repository. 

    :w 
    :! git add Gemfile
    :! git commit -am 'adding Gemfile'
  
Then push this to Heroku and it should download and install 
sinatra for you. After that the app should run. 

You can also run this application locally using the `thin` webserver.

    gem install thin 

Then install the bundle ( including sinatra ) locally. 

    bundle install 

Start the application and visit it at `0.0.0.0:3000`

    thin start

Yippee!!

	
