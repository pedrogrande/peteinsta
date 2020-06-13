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

- Go to Getting Started page of Getbootstrap.com and get the css CDN link and place in header of file
- Get JS links and paste at bottom of file before closing body tag </body>
<script src="https://kit.fontawesome.com/2fbcf4bc83.js" crossorigin="anonymous"></script>

- Change <body> tag to be the same as the HTML code from yesterday
- Copy across Navbar and Footer from HTML code from Day 1

>app/views/home/index.html.erb

- Copy across other code from index-3.html (or home.html)

## Users --> Authentication
> Gemfile

gem 'devise'
gem 'simpleform'

`bundle`




vagrant up
vagrant ssh
vagrant suspend
vagrant reload
