## Repo INFO

This project was remade and built on the original version at a later time, I had some issues with pulling and pushing files into the original repo. When the issue was noticed, I had to manually add each folder directly to the repo which caused the app to no longer work. Thus the project was moved to a new repo due to issues with pushing files to the original repo.

Original repo with outdated code and a LOT of errors: https://github.com/6hrslater/jungle-rails

# Jungle

A mini e-commerce application that allows users to purchase a variety of beautiful plants.

## Products Page

!["screenshot description"](https://github.com/6hrslater/jungle-rails-remake/blob/master/docs/products%20page.PNG)

## Item Info

!["screenshot description"](https://github.com/6hrslater/jungle-rails-remake/blob/master/docs/product%20info.PNG)

## Shopping Cart

!["screenshot description"](https://github.com/6hrslater/jungle-rails-remake/blob/master/docs/customer%20cart.PNG)

## Setup

1. Run `bundle install` to install dependencies
2. Create `config/database.yml` by copying `config/database.example.yml`
3. Create `config/secrets.yml` by copying `config/secrets.example.yml`
4. Run `bin/rails db:reset` to create, load and seed db
5. Create .env file based on .env.example
6. Sign up for a Stripe account
7. Put Stripe (test) keys into appropriate .env vars
8. Run `bin/rails s -b 0.0.0.0` to start the server

## Database

If Rails is complaining about authentication to the database, uncomment the user and password fields from `config/database.yml` in the development and test sections, and replace if necessary the user and password `development` to an existing database user.

## Stripe Testing

Use Credit Card # 4111 1111 1111 1111 for testing success scenarios.

More information in their docs: <https://stripe.com/docs/testing#cards>

## Dependencies

- Rails 6.1 [Rails Guide](http://guides.rubyonrails.org/v6.1/)
- Bootstrap 5
- PostgreSQL 9.x
- Stripe
