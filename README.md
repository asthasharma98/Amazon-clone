# Amazon Clone

Amazon Clone is the Fully functional Real custom made Web application that covers and entire E-commerece functionality from designing, User Authentication till Payments build using `React JS`, `Firebase` and `Stripe`.

- To view the deployed Application, click on the link given below : ***Amazon Clone Web App***  

### Features 

As a user you can 

- Login/Log out or set up a New Account(Register) 
- View list of different products 
- Add and remove them from Cart 
- proceed to checkout page to buy the product 
- create orders and Make payments 
- View Order history and details 

### Project Structure

Project consist of following stages:

- Setting up a react Router 
- creating the Navigation bar
- Creating the home Page of Amazon - to display sample products
- Setting up a React [Context API](https://reactjs.org/docs/context.html) - The Context API is a component structure provided by the React framework, which enables us to share specific states across all levels of the application. In this project, there is need to manage two states: basket (to manage the shopping cart) and user (for managing the details of the currently logged in user).
- Setting up payment functionality using API's provided by [Stripe](https://stripe.com/in)(Stripe is an online payment processing and credit card processing platform for businesses.)
- Setting up a [Firebase](https://firebase.google.com/) - for Handling database, authentication and also for depolying application.Basically the database will be used to store the login information for the users, but the resource can be used for storing product information as well.
- Setting up Authentication
- Deployement 

### Firebase 

Firebase is a great service provided by Google for configuring the backend of any web application with all the general necessities like database preparation, authentication using various methods, etc.

#### Setup

- Create a project on Firebase, setup the database and setup sign-in method using Email/Password.
- Register your application and set up Firebase hosting.
- nstall necessary Firebase dependencies in your local setup.
  ```
  npm install -g firebase-tools && npm install firebase && firebase login
  ```
- Open the `Firebase SDK snippet` section in your Firebase project and copy paste the necessary configuration in a file named `firebase.js`.
- In this file, utilize the below code to make use of Firebase authentication and database.
   ```
   const firebaseApp = firebase.initializeApp(firebaseConfig);

   const db = firebaseApp.firestore();
   const auth = firebase.auth();

   export { db, auth };
   ```
   
   **Reference link for above process is given below :**
   
   - [https://firebase.google.com/docs/web/setup](https://firebase.google.com/docs/web/setup)
   - [https://blog.logrocket.com/user-authentication-firebase-react-apps/](https://blog.logrocket.com/user-authentication-firebase-react-apps/)

 #### Deployment 
  
  - To deploy a production version of the Amazon Clone, we need to set up Firebase hosting. Type command in console
    ```
    npm init
    ```
  - Build your React application.
    ```
    npm run build
    ```
  - Setup Firebase hosting and deploy
    ```
    firebase deploy
    ```
  **Reference link for deploying application on firebase**
   - [https://firebase.google.com/docs/hosting/quickstart](https://firebase.google.com/docs/hosting/quickstart)
   - [https://medium.com/swlh/how-to-deploy-a-react-app-with-firebase-hosting-98063c5bf425](https://medium.com/swlh/how-to-deploy-a-react-app-with-firebase-hosting-98063c5bf425)
   
