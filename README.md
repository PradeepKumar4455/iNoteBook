# iNoteBook 📝
A MERN stack application to manage personal notes securely with authentication.  

## 🚀 Features
- User authentication (Signup/Login with JWT)  
- Create, Read, Update, Delete (CRUD) notes  
- Secure password hashing with bcrypt  
- Protected routes with JWT authentication  
- Responsive UI built with React  
- MongoDB as database  

## 🛠️ Tech Stack
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)
![Express](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)

## 📂 Project Structure
```
iNoteBook/
│
├── backend/          # Express + MongoDB code
│   ├── models/       # Mongoose schemas
│   ├── routes/       # API routes
│   ├── middleware/   # Auth middleware
|   ├── db.js         # MongoDB connection setup
│   └── index.js      # Main server file
│
|
├── Project_UI_Screenshots 
|
|
├── frontend/         # React app
│   ├── src/
│   │   ├── components/
│   │   ├── context/
│   │   ├── App.js
│   │   └── index.js
│
└── README.md
```

## ⚡ Installation & Setup

1. Clone the repository  
   ```bash
   git clone https://github.com/your-username/iNoteBook.git
   cd iNoteBook
   ```

2. Setup **backend**  
   ```bash
   cd backend
   npm install
   npm start
   ```

3. Setup **frontend**  
   ```bash
   cd frontend
   npm install
   npm start
   ```

4. Create a `.env` file in `backend/` and add:  
   ```
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_secret_key
   ```

## 📡 API Endpoints

### Auth Routes
- **POST** `/api/auth/createuser` → Register a new user  
- **POST** `/api/auth/login` → Login user & return auth token  
- **POST** `/api/auth/getuser` → Get logged-in user details (Requires Auth)  

### Notes Routes (Requires Auth)
- **GET** `/api/notes/fetchallnotes` → Fetch all notes of logged-in user  
- **POST** `/api/notes/addnote` → Add a new note  
- **PUT** `/api/notes/updatenote/:id` → Update an existing note  
- **DELETE** `/api/notes/deletenote/:id` → Delete a note  


## 🌐 Live Demo
👉 [Click here to view deployed app](https://your-deployment-link.com)  

## 📜 License
This project is licensed under the MIT License.  
