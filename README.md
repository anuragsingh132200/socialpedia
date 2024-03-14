
### MERN Social Media App

This project is a full-fledged social media application built using the MERN stack (MongoDB, Express.js, React.js, Node.js) with Redux for state management and React Router for navigation. It offers core social media functionalities, including:

- **User Authentication:** Secure login and registration for users.
- **User Profiles:** Customizable profiles with user information, posts, followers, and following lists.
- **Posts:** Create, view, edit, and delete posts, including text and image content.
- **Liking:** Like posts to express appreciation or agreement.
- **Commenting:** Leave comments on posts to participate in discussions.

**Project Structure:**

```
SOCIALPEDIA
├── .vscode
├── client
|  ├── public
|  ├── src
|  │   ├── QQUO
|  │   │   └── components
|  │   │       ├── FlexBetween.jsx
|  │   │       ├── Friend.jsx
|  │   │       └── Userlm
|  │   ├── scenes
|  │   │   ├── homePage
|  │   │   │   └── index.jsx
|  │   │   ├── loginPage
|  │   │   │   ├── Form.jsx
|  │   │   │   └── index.jsx
|  │   │   ├── navbar
|  │   │   │   └── index.jsx
|  │   │   ├── profilePage
|  │   │   │   └── index.jsx
|  │   │   └── widgets
|  │   │       ├── AdvertWidget.jsx
|  │   │       ├── FriendListWidget.jsx
|  │   │       ├── MyPostWidget.jsx
|  │   │       ├── PostsWidget.jsx
|  │   │       ├── PostWidget.jsx
|  │   │       └── UserWidget.jsx
|  │   ├── state
|  │   │   ├── index.js
|   │   │   ├── App.js
|  │   │   ├── index.css
|  │   │   ├── index.js
|  │   │   └── theme.js
|   │   └── ...
├── server/  (Node.js server)
│   ├── controllers/
│   │   ├── auth.js        (Authentication routes)
│   │   ├── posts.js        (Post management routes)
│   │   ├── users.js        (User management routes)
│   │   └── ...           (Other controllers)
│   ├── models/
│   │   ├── Post.js         (Post model)
│   │   ├── User.js         (User model)
│   │   └── ...           (Other models)
│   ├── routes/        (API routes)
│   │   ├── auth.js        (Authentication routes)
│   │   ├── posts.js        (Post management routes)
│   │   ├── users.js        (User management routes)
│   │   └── ...           (Other routes)
│   ├── server.js         (Primary server entry point)
│   └── middlewares/          (middleware functions)
│       ├── auth.js            (authentication middleware)
│       └── ...           (Other utility files)
└── README.md         (This file)
```

**Installation:**

1. Clone this repository.
2. Install dependencies:

   ```bash
   cd mern-socialpedia
   cd  server 
   npm install
   ```
   ```
   cd ../cleint 
   npm install
   ```

3. Create a `.env` file in the `backend` directory to store environment variables (MongoDB connection string, JWT secret, etc.).
4. (Optional) Set up a cloud storage service like Cloudinary for image uploads (refer to their documentation for specific steps).

**Running the Application:**

1. Start the backend server:

   ```bash
   cd backend
   node server.js
   ```

2. Start the frontend development server:

   ```bash
   cd client
   npm start
   ```

The application will typically be accessible at `http://localhost:3000/`.

**Additional Notes:**

- Consider implementing additional features like user search, notifications, messaging, privacy settings, and more.
- Thoroughly test all functionalities before deployment.
- Secure your application by following best practices for password hashing, input validation, and JWT authentication.
- Follow the guidelines of your chosen cloud storage service for secure image storage if applicable.

**Feel free to customize and extend this project to create a robust and engaging social media platform!**