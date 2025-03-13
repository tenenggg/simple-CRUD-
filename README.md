# ReactJS Firebase Realtime Database App

This is a web-based application built using **ReactJS** and **Firebase Realtime Database**. It allows users to perform CRUD (Create, Read, Update, Delete) operations on a collection of fruits stored in Firebase.

## Features
- **Write Data**: Users can add new fruit entries to Firebase.
- **Read Data**: Users can fetch and display fruit data from Firebase.
- **Update Data**: Users can modify existing fruit data.
- **Delete Data**: Users can remove fruit entries.

## Tech Stack
- **ReactJS**: Frontend framework
- **Firebase**: Realtime Database for data storage
- **React Router**: Navigation within the app
- **Dotenv**: Environment variables for Firebase configuration

## Installation & Setup
Follow these steps to set up and run the project on your local machine.

### 1. Clone the Repository
```sh
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### 2. Install Dependencies
```sh
npm install
```

### 3. Set Up Firebase
- Go to [Firebase Console](https://console.firebase.google.com/).
- Create a new project.
- Go to **Project Settings** > **General** > **Your apps**.
- Register your app and get Firebase config values.
- Enable Firebase Realtime Database in **Build** > **Realtime Database**.
- Set database rules to public for testing:
  ```json
  {
    "rules": {
      ".read": true,
      ".write": true
    }
  }
  ```

### 4. Create an `.env` File
Inside the project root, create a `.env` file and add your Firebase credentials:
```sh
REACT_APP_FIREBASE_API_KEY=your_api_key
REACT_APP_FIREBASE_AUTH_DOMAIN=your_auth_domain
REACT_APP_FIREBASE_DATABASE_URL=your_database_url
REACT_APP_FIREBASE_PROJECT_ID=your_project_id
REACT_APP_FIREBASE_STORAGE_BUCKET=your_storage_bucket
REACT_APP_FIREBASE_MESSAGING_SENDER_ID=your_messaging_sender_id
REACT_APP_FIREBASE_APP_ID=your_app_id
REACT_APP_FIREBASE_MEASUREMENT_ID=your_measurement_id
```

### 5. Start the Project
```sh
npm start
```
This will start the development server at `http://localhost:3000/`.

## Project Structure
```
📁 your-repo-name
├── 📁 src
│   ├── 📁 components
│   │   ├── Write.js  # Component to add data
│   │   ├── Read.js  # Component to read data
│   │   ├── UpdateRead.js  # Component to update and delete data
│   │   ├── UpdateWrite.js  # Component to edit data
│   ├── firebaseConfig.js  # Firebase configuration file
│   ├── App.js  # Main app component with routes
├── .env  # Environment variables (ignored in Git)
├── package.json  # Dependencies and scripts
├── README.md  # Project documentation
```

## Tutorials & References
- **Firebase Setup**: [Firebase Web Docs](https://firebase.google.com/docs/web/setup)
- **React Router**: [React Router Docs](https://reactrouter.com/en/main)
- **React with Firebase**: [Firebase React Guide](https://firebase.google.com/docs/database/web/start)

## Contributing
Feel free to fork the project and submit pull requests!

## License
This project is licensed under the MIT License.

