# Tshirt store API

It's an API for Tshirt ecommerce store with functionality of user signup, login using jwt, logout and with custom roles for example Admin with power to update user's details, product's details and can manage various things in the database.

### Hosted link: [Tshirt store api](https://buy-tshirt-api.onrender.com/api/v1)

### Documentation : [Api documentation](https://buy-tshirt-api.onrender.com/api-docs/)

## Installation Guide

- Clone this repository
- Run npm install to install all the dependencies
- You can either work with MongoDB atlas or use your locally installed MongoDB
- Create a .env file in your project root folder and add your variables.

---

## Please add env variables for the project

#### PORT=4000

#### DB_URL=

#### JWT_SECRET=

#### JWT_EXPIRY=

#### COOKIE_TIME=

#### CLOUDINARY_NAME=

#### CLOUDINARY_API_KEY=

#### CLOUDINARY_API_SECRET=

#### SMTP_HOST=

#### SMTP_PORT=

#### SMTP_USER=

#### SMTP_PASS=

#### STRIPE_API_KEY=

#### STRIPE_SECRET=

#### RAZORPAY_API_KEY=

#### RAZORPAY_SECRET=

---

## Features

### User

- Signup
- Login
- Logout
- Forgot password

### Admin

- Update user
- Delete user
- Add product
- Update product
- Delete product
- Update order
- Delet order

### Product

- All products
- Single product
- Reviews
- Post review (logged in user)
- Delete review (logged in user)

### Order

- Create order
- Details about an order
- Orders of logged in user

### Payment

- Stripe payment
- Razorpay payment

---

## API Endpoints

| HTTP Verbs | Endpoints                    | Action                                         |
| ---------- | ---------------------------- | ---------------------------------------------- |
| POST       | api/v1/signup                | To sign up a new user account                  |
| POST       | api/v1/login                 | To login an existing user account              |
| GET        | api/v1/logout                | To logout logged in user                       |
| POST       | api/v1/forgotPassword        | To send and email with link to forgot password |
| POST       | api/v1/password/reset/:token | To allow user to reset password                |
| GET        | api/v1/userDashboard         | To get all the details of the logged in user   |
| POST       | api/v1/password/update       | To update password (logged in user)            |
| POST       | api/v1/userdashboard/update  | To update user details (logged in user)        |
| GET        | api/v1/admin/users           | To get all the users                           |
| GET        | api/v1/admin/users/:id       | To get detail of an user                       |
| PUT        | api/v1/admin/users/:id       | To update an user                              |
| DELETE     | api/v1/admin/users/:id       | To delete an user                              |
| GET        | api/v1/admin/products        | To get all the products                        |
| POST       | api/v1/admin/product/add     | To add a product                               |
| PUT        | api/v1/admin/product/:id     | To update a product                            |
| DELETE     | api/v1/admin/product/:id     | To delete a product                            |
| GET        | api/v1/admin/orders          | To get list of orders                          |
| PUT        | api/v1/admin/order/:id       | To update status of order                      |
| DELETE     | api/v1/admin/order/:id       | To delete an order                             |
| GET        | api/v1/products              | To get all available products                  |
| GET        | api/v1/product/:id           | To get a single product                        |
| GET        | api/v1/reviews               | To get all review of a given product           |
| PUT        | api/v1/review                | To post/update an review (logged in user)      |
| DELETE     | api/v1/review                | To delete an review (logged in user)           |
| POST       | api/v1/order/create          | To create a new order with given details       |
| GET        | api/v1/order/:id             | To get details about an order with order id    |
| GET        | api/v1/myorder               | To get orders of logged in user                |
| GET        | api/v1/stripekey             | To get public stripe key                       |
| GET        | api/v1/razorpaykey           | To get public razorpay key                     |
| POST       | api/v1/capturestripe         | To send amount in number                       |
| POST       | api/v1/capturestripe         | To send amount in number                       |

___

## Technologies used

- NodeJs
- ExpressJs
- MongoDB
- Mongoose ODM

