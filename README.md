# ar-on-web

# Three.js Website with Firebase Storage and Firebase Hosting

This repository contains the code for a Three.js website that utilizes Firebase Storage for storing assets and Firebase Hosting for deployment. By following the instructions below, you will be able to clone the repository, set up the required Firebase services, and run the website locally or deploy it to Firebase Hosting.

## Prerequisites

Before getting started, ensure that you have the following:

- Git installed on your local machine.
- Node.js and npm (Node Package Manager) installed.

## Clone the Repository

To clone the repository, open your terminal or command prompt and execute the following command:

```bash
git clone https://github.com/your-username/threejs-website.git
```

Replace `your-username` with your GitHub username or provide the appropriate URL to the repository.

## Firebase Setup

To use Firebase Storage and Firebase Hosting, follow these steps:

### Create a Firebase Project

1. Visit the [Firebase Console](https://console.firebase.google.com/).
2. Click on "Add project" or select an existing project.
3. Provide a project name and select your desired options.
4. Click on "Create project".

### Set Up Firebase Storage

1. In the Firebase Console, navigate to your project.
2. Click on "Storage" in the left menu.
3. Click on "Get started" and follow the instructions to set up Firebase Storage.
4. Note down your Firebase Storage bucket URL.

### Set Up Firebase Hosting

1. In the Firebase Console, navigate to your project.
2. Click on "Hosting" in the left menu.
3. Click on "Get started" and follow the instructions to set up Firebase Hosting.
4. Note down your Firebase Hosting domain.

### Configure the Website

1. Open the cloned repository in your preferred code editor.
2. Locate the file `firebase-config.js` in the root directory.
3. Replace the placeholders with your Firebase project configuration details. The file should look like this:

   ```javascript
   export const firebaseConfig = {
     apiKey: 'YOUR_API_KEY',
     authDomain: 'YOUR_AUTH_DOMAIN',
     databaseURL: 'YOUR_DATABASE_URL',
     projectId: 'YOUR_PROJECT_ID',
     storageBucket: 'YOUR_STORAGE_BUCKET',
     messagingSenderId: 'YOUR_MESSAGING_SENDER_ID',
     appId: 'YOUR_APP_ID',
   };
   ```

4. Save the file.

## Run the Website Locally

To run the website on your local machine, follow these steps:

1. Open your terminal or command prompt.
2. Navigate to the cloned repository's directory.
3. Run the following command to install the project dependencies:

   ```bash
   npm install
   ```

4. After the installation is complete, run the following command to start the local development server:

   ```bash
   npm start
   ```

5. Open your web browser and visit `http://localhost:3000` to see the website in action.

## Deploy to Firebase Hosting

To deploy the website to Firebase Hosting, follow these steps:

1. Open your terminal or command prompt.
2. Navigate to the cloned repository's directory.
3. Run the following command to build the website for production:

   ```bash
   npm run build
   ```

4. Once the build process is finished, run the following command to deploy to Firebase Hosting:

   ```bash
   firebase deploy
   ```

5. Firebase will provide you with the deployed URL. Open your web browser and visit the provided URL to see your deployed website.

## Contributing

Feel free to contribute to this project by submitting bug reports, feature requests, or pull requests on the GitHub repository.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowled

gments

- The Three.js framework: [https://threejs.org/](https://threejs.org/)
- Firebase: [https://firebase.google.com/](https://firebase.google.com/)
