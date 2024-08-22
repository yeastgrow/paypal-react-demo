[![en](https://img.shields.io/badge/lang-en-green.svg)](https://github.com/yeastgrow/paypal-react-demo/blob/master/README.md)
[![zh](https://img.shields.io/badge/lang-zh-red.svg)](https://github.com/yeastgrow/paypal-react-demo/blob/master/README.zh.md)


# Introduction

- Welcome to the frontend repository of our project, which is designed to complement the backend project [paypal-springboot-demo](https://github.com/yeastgrow/paypal-springboot-demo). This project serves two main purposes:

 1. **Purpose 1**: To summarize the mainstream payment API types and their usage logic.
 2. **Purpose 2**: To serve as a sandbox for testing different scenarios and issues.

- This project was initially derived from the PayPal official [demo](https://codeload.github.com/paypaldev/PayPal-JavaScript-FullStack-Standard-Checkout-Sample/zip/refs/heads/main). 
- The backend of the official project was originally in Node.js, but this project has been adapted to work with a [Java Spring Boot](https://github.com/yeastgrow/paypal-springboot-demo) backend. 
- For detailed invocation process documentation, please refer to the [paypal-springboot-demo](https://github.com/yeastgrow/paypal-springboot-demo) project.

- PayPal API Integrations:
  The project integrates several core PayPal APIs to facilitate a wide range of payment operations:
  1. Orders and Payments: Manage orders and process payments efficiently. 
  2. Subscriptions: Handle recurring payments with ease. 
  3. Invoices: Create and send invoices to customers. 
  4. Disputes: Address and manage disputes that may arise.

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

This project is designed to work seamlessly with the backend, which you can find at [paypal-springboot-demo](https://github.com/yeastgrow/paypal-springboot-demo). Below are the steps to get your frontend running locally.


### Prerequisites

Before you begin, ensure you have met the following requirements:
- Node.js and npm installed on your machine.
- Basic understanding of JavaScript and React.

Follow these steps to install and run the frontend project on your local machine.

### Step 1: Clone the Repository

Clone the project repository to your local machine using:

```bash
git clone https://github.com/your-username/your-repo-name.git
```

### Step 2: Install Dependencies

Navigate to the project directory and run:

```bash
npm install
```

### Step 3: Set Up PayPal Client ID

In the `client/App.jsx` file, locate the `initialOptions` object and enter your PayPal `client-id`.

### Step 4: Configure Backend Connection

Modify the backend port information in the `vite.config.js` file to match your backend setup.

### Step 5: Start the Development Server

Run the following command in the project root directory to start the frontend:

```bash
npm run client-dev
```

### Step 6: Access the Application

Open your web browser and navigate to `http://localhost:3000/` to view the frontend.



We hope this project helps you understand and test PayPal APIs effectively. Feel free to contribute and provide feedback!