# Secrets-app

**Share your secrets anonymously!**  
A full-stack web app built with Node.js, Express, and MongoDB that allows users to register, log in, and share secrets anonymously. Features local authentication, Google OAuth, session management, and secret sharing.

---

## 🚀 Features

- **User Registration and Login** (local and Google OAuth)
- **Anonymous Secret Submission**
- **Secrets List:** View all submitted secrets (without user identity)
- **Session Management:** Persistent login and logout
- **MongoDB Integration:** Stores user credentials and secrets securely
- **Password Encryption:** Utilizes Passport.js, bcrypt, mongoose-encryption
- **Responsive EJS Views** (home, register, login, submit, secrets)

---

## 📁 Project Structure
```
/
├── app.js # Main application file
├── package.json # Project dependencies and scripts
├── views/ # EJS templates
│ ├── home.ejs
│ ├── login.ejs
│ ├── register.ejs
│ ├── secrets.ejs
│ └── submit.ejs
├── public/ # Static assets (CSS, images)
└── .gitignore
```

---

## 🛠️ Tech Stack

- **Backend:** Node.js, Express.js
- **Frontend:** EJS templating, HTML, CSS
- **Database:** MongoDB & Mongoose
- **Authentication:** Passport.js (`local`, `Google`, `GitHub`)
- **Environment:** dotenv for secret keys

---

## 🔧 Setup Instructions

### 1. Clone the repository

```
git clone https://github.com/abo-ah-md/Secrets-app.git
cd Secrets---Starting-Code
```

### 2. Install dependencies
```
npm install
```

### 3. Set up environment variables

Create a `.env` file in the root directory with your Google OAuth keys:

```
CLIENT_ID=your-google-client-id
CLIENT_SECRET=your-google-client-secret
```

### 4. Start MongoDB

Ensure MongoDB is running locally (default URI: `mongodb://localhost:27017/UsersDB`).

### 5. Start the app

```
node app.js
```
App runs on `http://localhost:3000`

---

## 🔑 Usage

- **Home page:** `/` — Project description, Register/Login buttons
- **Register:** `/register` — Create a user account
- **Login:** `/login` — Log in via local credentials or Google OAuth
- **Submit Secret:** `/submit` — Submit a secret (must be authenticated)
- **View Secrets:** `/secrets` — Anonymous secrets list
- **Logout:** `/logout` — End session

---

## 📦 Dependencies

Major NPM packages:

- `express`, `body-parser`, `ejs`
- `mongoose`, `mongoose-encryption`, `mongoose-findorcreate`
- `passport`, `passport-local`, `passport-local-mongoose`, `passport-google-oauth20`, `passport-github2`
- `express-session`, `dotenv`, `bcrypt`, `md5`, `cookie-parser`

See `package.json` for a full list.

---

## 📜 License

ISC License (see `package.json`)

---

## 🙌 Credits

Created by **abo-ah-md**.  
Inspired by Angela Yu's Web Development Bootcamp project.
