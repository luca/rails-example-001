## Demo application for [GetProductionReady](http://getproductionready.com)

This is one of the demo applications used for my [GetProductionReady](http://getproductionready.com) mailing list.

It's just a basic "blog"-like application with a scaffolded Post entity.

It uses the Figaro gem to handle application settings.

To run it:


1. run ```bundle``` to install the gems
2. create the application.yml file if you didn't have one: 
```
echo "SECRET_TOKEN: `rake secret`" > config/application.yml
```
3. create the database.yml file
4. create the database & migrate:
```
bundle exec rake db:create:all
bundle exec rake db:migrate
```
5. run the server: 
```
bundle exec rails server
```