# Introduction

- Welcome to the frontend repository of our project, which is designed to complement the backend project [paypal-springboot-demo](https://github.com/yeastgrow/paypal-springboot-demo). This project serves two main purposes:

 1. **Purpose 1**: To summarize the mainstream payment API types and their usage logic.
 2. **Purpose 2**: To serve as a sandbox for testing different scenarios and issues.

- This project was initially derived from the PayPal official [demo](https://codeload.github.com/paypaldev/PayPal-JavaScript-FullStack-Standard-Checkout-Sample/zip/refs/heads/main). 
- The backend of the official project was originally in Node.js, but this project has been adapted to work with a [Java Spring Boot](https://github.com/yeastgrow/paypal-springboot-demo) backend. 
- For detailed invocation process documentation, please refer to the [paypal-springboot-demo](https://github.com/yeastgrow/paypal-springboot-demo) project.

- The main PayPal APIs that will be covered in this project include:
 1. **Order + Payment**
 2. **Subscriptions**
 3. **Invoices**
 4. **Disputes**

## Using Sandbox

To get started with testing, you need to:

- Create a PayPal developer account [here](https://developer.paypal.com/dashboard/accounts/).
- Each developer account comes with two default test accounts: one personal (for simulating the payer's behavior) and one business (for simulating the merchant's behavior).
  - Access these accounts through the developer dashboard: `developer account -> testing tool -> sandbox account`.
    - **Personal**: Includes Name, Phone, Country, Account ID, Email, and Password.
    - **Business**: Includes Client ID, Secret, Name, Phone, Country, Account ID, Email, and Password.
- During programming tests, you can log in to the [sandbox](https://www.sandbox.paypal.com/mep/dashboard) test account to view the account dashboard and balance.
- Each sandbox account is initially funded with $5000.

## Running the Frontend Project

To run the frontend project, follow these steps:

1. Rename the file `.env.example` to `.env`.
2. Add the necessary environment variables to the `.env` file.
3. Install the frontend dependencies by running `npm install`.
4. In the `client/App.jsx` file, locate the `initialOptions` object and enter your PayPal `client-id`.
5. Modify the backend port information in the `vite.config.js` file.
6. Start the frontend by running `npm run client-dev` in the project root directory.
7. Open your browser and navigate to `http://localhost:3000/`.

We hope this project helps you understand and test PayPal APIs effectively. Feel free to contribute and provide feedback!