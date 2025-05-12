# lab_three_api

A Ruby on Rails application in API mode for Lab Three.

## Features

- User 1:M Post association
- Creator association: Post belongs to a creator (User)
- Post M:M Editor association via custom join table (no HABTM)
- CRUD APIs for Users and Posts
- Postman collection included (exported as JSON)

## Setup

```bash
git clone https://github.com/your-username/lab_three_api.git
cd lab_three_api
bundle install
rails db:create db:migrate db:seed
rails s
