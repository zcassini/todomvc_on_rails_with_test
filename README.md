# TodoMVC on Rails

### Built by Matt De Leon
He built the TodoMVC app according to its spec using only Rails 4 and a hint of javascript. See his article for more details
http://www.mattdeleon.net/

### Tests added by [@kashiro](https://github.com/kashiro)
He updated it to learn how to create unit tests using RSpec and feature tests using Capybara


# Update
This app has been updated to make sure it runs on the Free Code Camp zeus vagrant ruby box.

## Installation
1. Clone the repo:
```
git clone https://github.com/zcassini/todomvc_on_rails_with_test.git
```

2. Create the development database:
```
bin/create-pg-app-db fcctodomvc_dev
```
Use `fcctodomvc_dev` for the password

3. Create the test database:
```
bin/create-pg-app-db fcctodomvc_test  
```
Use `fcctodomvc_test` for the password

4. Initialize the the databases:
```
bundle exec rake db:migrate
bundle exec rake db:migrate RAILS_ENV=test
```

5. Run the tests
```
xvfb-run -a bundle exec rspec
```

6. Start the rails server
```
rails s
```
or if using the vagrant box use
```
rails s -b 0.0.0.0
```

7. Enjoy http://localhost:3000
