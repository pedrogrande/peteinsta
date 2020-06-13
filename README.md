# Instruction steps


## Create home page and set to root route
rails g controller home index
> config/routes.rb

root "home#index"

## Add Bootstrap and Fontawesome gems

>app/assets/stylesheets/application.css
rename to application.scss
Delete contents

>app/views/layouts/application.html.erb

- Go to Getting Started page of Getbootstrap.com and get the css CDN link and place in `<head>`
- Get JS links and paste at bottom of file before closing body tag `</body>`
- Fontawesome put in `<head>`: <script src="https://kit.fontawesome.com/2fbcf4bc83.js" crossorigin="anonymous"></script>

- Change `<body>` tag to be the same as the HTML code from yesterday
- Copy across Navbar and Footer from HTML code from Day 1

>app/views/home/index.html.erb

- Copy across other code from index-3.html (or home.html)

## Users --> Authentication
> Gemfile

- gem 'devise'
- gem 'simple_form'

- `bundle`
- stop server
- `rails g devise:install`
- `rails g devise User`
- `rails db:migrate`
- `rails g simple_form:install --bootstrap`
- `rs`

## General shell/terminal commands
- `ls` (lists files in current directory)
- `pwd` (present working directory)
- `whoami` (what user am i at the moment)
- `cd [directory name]/[other directory name]` (change into this directory/subdirectory)
- `cd ..` (change into the directory above the current directory)
- `cd ~` (go to home directory)
- Control+C (stop server running/cancel operation)

## Vagrant commands
- `vagrant up`
- `vagrant ssh`
- `vagrant suspend`
- `vagrant reload`

## Rails commands
- `rs` (normally `rails s` but in this vagrant environment it is an alias for `rails s -b 0.0.0.0`)
- `bundle` (After editing Gemfile, this command needs to be run and the server needs to be restarted)
- `rails db:migrate` (Make changes to database - run migration files)
- 
