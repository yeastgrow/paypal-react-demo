# 1. 大致介绍
- 该项目是项目[paypal-springboot-demo](https://github.com/yeastgrow/paypal-springboot-demo) 的前端项目，该项目主要有两个目的
  - 目的 1：归纳主流支付api类型和使用逻辑的梳理。
  - 目的 2：用作 sandbox，对不同的场景和问题进行测试
- 该项目是由paypal官网[demo](https://codeload.github.com/paypaldev/PayPal-JavaScript-FullStack-Standard-Checkout-Sample/zip/refs/heads/main)为初始项目进行修改
    - 官网项目的后端使用的是 Node，该项目适配的是 [java springboot](https://github.com/yeastgrow/paypal-springboot-demo)的后端
    - 具体的调用流程整理请参见项目 [paypal-springboot-demo](https://github.com/yeastgrow/paypal-springboot-demo)
- 主要会涉及介绍的 paypal API
1. order + payment
2. Subscriptions
3. Invoices
4. Disputes

# 2. 使用 Sandbox

- 开通 PayPal developer 的一个 account [link](https://developer.paypal.com/dashboard/accounts/) 
- 每个 developer 账号下面会默认给两个测试账号，一个是个人测试账号（用于模仿付款方行为），一个是企业账号（用于模仿商户行为）
  - developer account -> testing tool -> sandbox account
    - personal: Name,Phone, Country, Account ID, email, ps
    - business: clientId, secret, Name,Phone, Country, Account ID, email, ps
- 在编程测试过程中可以登录 [sandbox](https://www.sandbox.paypal.com/mep/dashboard) 的测试账户查看账户面板和账户中的金额 
- 每个sandbox账号都有初始 5000刀的金额

# 3. 跑前端项目

- 修改文件名 `.env.example` 为 `.env`.
- 在其中加入所需要的环境变量
- 安装前端所需的依赖  `npm install`.
- 在`client/App.jsx` 文件中，找到 `initialOptions` 对象，输入你 Paypal 的 `client-id`
- 修改 `vite.config.js` 文件中后端端口的信息
- 在项目跟目录，启动前端 `npm run client-dev`
- 打开你的浏览器 `http://localhost:3000/`


