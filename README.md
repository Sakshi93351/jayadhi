

### Conversa is a chat-app with various features like:
-    **Authentication**:  
     SignUp,  
     Login,  
     Login with OTP,  
     Profile Photo Uploading.
    
-    **Styling/Theming**:  
     A fully responsive app,  
    🌙 Dark and ☀️ Light mode.
    
-    **Personalized AI Chatbot**:  
     Remembers the context for personalized interactions.
    
-    **Web Sockets**:  
     Real-time chatting,  
     Message Notifications,  
     Real-Time Typing Animation,  
     Message Deletion,  
     Active Now /  Last Seen status tracking,  
     Message Seen status,  
    🖼 Sending Image messages with captions.


	

```
username : guestuser1@gmail.com, guestuser2@gmail.com
password: 1234guest
```

---

## 🔗 Table of Contents

- [📍 Overview](#-overview)
- [👾 Features](#-features)
- [📁 Project Structure](#-project-structure)
  - [📂 Project Index](#-project-index)
- [🚀 Getting Started](#-getting-started)
  - [☑️ Prerequisites](#-prerequisites)
  - [⚙️ Installation](#-installation)
  - [🤖 Usage](#-🤖usage)
  - [🧪 Testing](#-🧪testing)
- [📌 Project Roadmap](#-project-roadmap)
- [🔰 Contributing](#-contributing)
- [🎗 License](#-license)
- [📝 About the Author](#-about-the-author)
- [🙌 Acknowledgments](#-acknowledgments)

---

## 📍 Overview

The MERN-Chat-App is a cutting-edge solution designed to streamline real-time communication. It leverages the MERN stack (MongoDB, Express.js, React, and Node.js) to offer a robust, scalable chat application. Key features include real-time communication with features like other trending social media applications and seamless integration with cloud services like AWS S3, Google Cloud's AI.


   
  

## 👾 Features

|      | Feature         | Summary       |
| :--- | :---:           | :---          |
| ⚙️  | **Architecture**  | <ul><li>Utilizes a MERN stack, integrating MongoDB, Express.js, React, and Node.js.</li><li>Backend designed to interact with cloud services like AWS S3 and Google Cloud's AI services.</li><li>Microservices architecture potential, suitable for scalable, distributed systems.</li></ul> |
| 🔩 | **Code Quality**  | <ul><li>Structured project with separate directories for backend and frontend.</li><li>Consistent use of JavaScript across the project.</li><li>Includes a `secrets.js` for managing environment variables, enhancing maintainability.</li></ul> |
| 📄 | **Documentation** | <ul><li>Documentation includes detailed install and usage commands.</li><li>Usage of badges in documentation for visual enhancement and clarity.</li><li>Language distribution shows a heavy use of JavaScript, ensuring consistency.</li></ul> |
| 🔌 | **Integrations**  | <ul><li>Integrates with npm for package management.</li><li>Backend interacts with AWS S3 and Google Cloud services.</li><li>Potential for integration with other cloud-based services or APIs due to its flexible backend.</li></ul> |
| 🧩 | **Modularity**    | <ul><li>Clear separation between frontend and backend codebases.</li><li>Modular structure aids in the maintainability and scalability of the project.</li><li>Use of JSON for configuration and inter-component communication enhances modularity.</li></ul> |
| 🧪 | **Testing**       | <ul><li>Includes npm scripts for testing, though detailed testing strategies are not specified.</li><li>Use of `npm test` suggests integration with JavaScript testing frameworks.</li><li>Testing likely focuses on backend services given the project's structure.</li></ul> |
| ⚡️  | **Performance**   | <ul><li>Use of Node.js and React suggests a focus on high-performance, non-blocking I/O operations.</li><li>Cloud integrations imply readiness for high-load environments.</li><li>Efficient dependency management through `package-lock.json` ensures consistent performance across environments.</li></ul> |
| 🛡️ | **Security**      | <ul><li>Management of secrets via `secrets.js` enhances security.</li><li>Dependency on secure cloud services like AWS S3 and Google Cloud.</li><li>Further security practices and configurations are not detailed but are crucial for future development.</li></ul> |
| 📦 | **Dependencies**  | <ul><li>Heavy reliance on npm for both frontend and backend dependencies.</li><li>Use of `package-lock.json` to lock down versions for consistency.</li><li>Dependencies suggest a robust setup with cloud services integration.</li></ul> |

---

## 📁 Project Structure

```sh
└── mern-chat-app/
    ├── LICENSE
    ├── README.md
    ├── backend
    │   ├── Controllers
    │   │   ├── auth_controller.js
    │   │   ├── conversation_controller.js
    │   │   ├── message_controller.js
    │   │   └── userController.js
    │   ├── Models
    │   │   ├── Conversation.js
    │   │   ├── Message.js
    │   │   └── User.js
    │   ├── README.md
    │   ├── Routes
    │   │   ├── auth_routes.js
    │   │   ├── conversation_routes.js
    │   │   ├── message_routes.js
    │   │   └── userRoutes.js
    │   ├── config
    │   │   └── imageupload.js
    │   ├── db.js
    │   ├── index.js
    │   ├── middleware
    │   │   └── fetchUser.js
    │   ├── package-lock.json
    │   ├── package.json
    │   ├── secrets.js
    │   ├── socket
    │   │   ├── handlers.js
    │   │   └── index.js
    │   └── uploads
    │       └── a
    ├── frontend
    │   ├── README.md
    │   ├── netlify.toml
    │   ├── package-lock.json
    │   ├── package.json
    │   ├── public
    │   │   ├── android-chrome-192x192.png
    │   │   ├── android-chrome-512x512.png
    │   │   ├── apple-touch-icon.png
    │   │   ├── favicon-16x16.png
    │   │   ├── favicon-32x32.png
    │   │   ├── favicon.ico
    │   │   ├── index.html
    │   │   ├── manifest.json
    │   │   └── robots.txt
    │   └── src
    │       ├── App.css
    │       ├── App.js
    │       ├── App.test.js
    │       ├── assets
    │       │   └── newmessage.wav
    │       ├── components
    │       │   ├── Authentication
    │       │   ├── Dashboard
    │       │   ├── Home.js
    │       │   ├── Navbar
    │       │   └── miscellaneous
    │       ├── context
    │       │   ├── appState.js
    │       │   └── chatContext.js
    │       ├── index.css
    │       ├── index.js
    │       ├── reportWebVitals.js
    │       ├── setupTests.js
    │       └── typingAnimation.json
    └── screenshots
        ├── 10_login_otp.png
        ├── 1_home.png
        ├── 2_login_signup.png
        ├── 3_dashboard.png
        ├── 4_newchat.png
        ├── 5_searching.png
        ├── 6_chatting_area.png
        ├── 7_send_photo.png
        ├── 8_delete_message.png
        ├── 9_login_otp.png
        ├── banner.png
        ├── new_message.png
        ├── personal_chatbot.png
        └── typing_animation.png
```


### 📂 Project Index

		

The dependencies listed within this file suggest that the backend is designed to interact with various cloud services, notably AWS S3 for storage solutions and Google Cloud's Vertex AI and Generative AI for advanced computational and AI-driven tasks<br>- This setup indicates a robust, scalable backend architecture that leverages leading cloud technologies for data handling and AI functionalities.

In the broader context of the project, this file ensures that the backend's dependency management is stable and predictable, which is crucial for maintaining the reliability and efficiency of the system as it interacts with cloud services and handles complex operations<br>- This is especially important in a microservices architecture or in a scenario where continuous integration and deployment are practiced, as it helps in reducing conflicts during deployments and across team environments.sensitive data is not hard-coded but instead dynamically referenced throughout the application's backend architecture.</td>
			
							
## 🚀 Getting Started

### ☑️ Prerequisites

Before getting started with mern-chat-app, ensure your runtime environment meets the following requirements:

- **Version Controller** Git
- **Programming Language:** JavaScript/Node.js
- **Package Manager:** Npm

### ⚙️ Installation

Install chat-app using one of the following methods:

**Build from source:**

1. Clone the mern-chat-app repository:
	```
	git clone https://github.com/Sakshi93351/jayadhi
	```

2. Navigate to the project directory:
	```
	cd jayadhi
	```

3. Setup Backend
	- Install Dependencies
	    ```
	    cd backend
	    npm install
	    ```
   - Setup Environment: Create a **.env** file in the backend folder and add necessary environment variables.
	    ```
	    PORT=5000
	    GENERATIVE_API_KEY = ""
	    MONGO_URI = ""
	    EMAIL = ""
	    PASSWORD= ""
	    CLOUDINARY_ClOUD_NAME = ""
	    CLOUDINARY_API_KEY = ""
	    CLOUDINARY_API_SECRET = ""
	    JWT_SECRET = ""
	    AWS_ACCESS_KEY = ""
	    AWS_SECRET = ""
	    AWS_BUCKET_NAME = ""
	    ```
    
4. Setup Frontend
	- Install Dependencies
	    ```
	    cd frontend
	    npm install
	    ```

### 🤖 Usage
Run mern-chat-app using the following command:
**Using `npm`** &nbsp; [<img align="center" src="https://img.shields.io/badge/npm-CB3837.svg?style={badge_style}&logo=npm&logoColor=white" />](https://www.npmjs.com/)

1. Start the backend server:
    ```
    cd backend
    nodemon ./index.js
    ```
2. Start the frontend development server:
    ```
    cd frontend
    npm run start
    ```
---
## 📌 Project Roadmap

- [X] **`Delete`**: <strike>Add Delete Message Feature</strike>
- [ ] **`Reply`**: Add reply to features.
- [ ] **`Reaction`**: Add message reactions.

---


<details closed>
<summary>Contributing Guidelines</summary>

1. **Fork the Repository**: Start by forking the project repository to your github account.
2. **Clone Locally**: Clone the forked repository to your local machine using a git client.
   ```sh
   git clone GitHub - Sakshi93351/jayadhi
   ```
3. **Create a New Branch**: Always work on a new branch, giving it a descriptive name.
   ```sh
   git checkout -b new-feature-x
   ```
4. **Make Your Changes**: Develop and test your changes locally.
5. **Commit Your Changes**: Commit with a clear message describing your updates.
   ```sh
   git commit -m 'Implemented new feature x.'
   ```
6. **Push to github**: Push the changes to your forked repository.
   ```sh
   git push origin new-feature-x
   ```
7. **Submit a Pull Request**: Create a PR against the original project repository. Clearly describe the changes and their motivations.
8. **Review**: Once your PR is reviewed and approved, it will be merged into the main branch. Congratulations on your contribution!


## 🎗 License

This project is licensed under the MIT License and Free to use.

## 📝 About the Author
This project was developed by  me (**Sakshi Prajapati**). Feel free to reach out with any questions or suggestions.
- gmail – sakshiprajapati9335@gmail.com
- kaggle - https://www.kaggle.com/sakshi


## 🙌 Acknowledgments

- List any resources, contributors, inspiration, etc. here.
