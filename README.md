Rails Todo API to interact with React Front-End Website @ https://github.com/brandoncabael/react-todo-web

## Table of Contents
- [Installation Non Docker](#installation-non-docker)
- [Installation Docker](#installation-docker)

## Installation Non Docker
Use RVM or other ruby version manager to install ruby-2.5.0

Install rails gem
`gem install rails`

Install bundler gem
`gem install bundler`

Clone repo to local folder
`git clone https://github.com/brandoncabael/rails-todo-api.git`

Install gem dependencies
`bundle install`

Run db migrate
`rails db:migrate`

Start development server
`rails server`

API should be running on http:localhost:3000 for React Front-End to interact with.

## Installation Docker
Clone repo to local folder
`git clone https://github.com/brandoncabael/rails-todo-api.git`

Build docker image
`docker build -t todos-api .`

Run docker image
`docker run -it -v ${PWD}:/app -p 3000:3000 --rm todos-api`

API should be running on http:localhost:3000 for React Front-End to interact with.