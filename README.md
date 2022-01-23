# demo_flutter_stripe_pay_gateway
This is a Simple demonstration on how to integrate Stripe Payment Gateway in a Flutter App

## To Run this App

- Install the dependencies
  - `flutter pub get`
- Set up env vars for the flutter app and a local backend.
  - [Get your test Stripe API keys](https://stripe.com/docs/keys)
  - `cp lib/.envX.dart lib/.env.dart` and set your Stripe publishable key.
  - `cp server/.env.example server/.env` and set the variable values in your newly created `.env` file.
- Install the server dependencies: `yarn --cwd "server"`
- Start the example
  - Terminal 1: `yarn --cwd "server" start`
  - Terminal 2: `flutter run`

##### Additional steps for webhook forwarding

- [Install the `stripe-cli`](https://stripe.com/docs/stripe-cli)
- Run `stripe listen --forward-to localhost:4242/webhook`
