Permalist – Task Manager App

A simple and powerful task management web application built using Node.js, Express, PostgreSQL, and EJS. This app allows users to add, edit, and delete daily tasks efficiently.

🚀 Features

✅ Add new tasks

✏️ Edit existing tasks

🗑️ Delete tasks

💾 Data stored securely using PostgreSQL

⚡ Fast and responsive UI

🔁 Live reload using Nodemon

🛠️ Technologies Used

Node.js

Express.js

PostgreSQL

pg (Postgres Client)

EJS (Embedded JavaScript Templates)

HTML, CSS

Nodemon

📂 Project Structure
Permalist/
│
├── public/            # Static files (CSS, images)
├── views/             # EJS templates
├── node_modules/      # Installed packages
├── index.js        # Main server file
├── queries.sql        # Database queries (ignored in Git)
├── .env               # Environment variables (ignored)
├── .gitignore
├── package.json
└── README.md

🧑‍💻 Installation & Setup
1️⃣ Clone the repository
git clone https://github.com/Surya1217/permalist.git
cd permalist

2️⃣ Install dependencies
npm install

3️⃣ Set up PostgreSQL Database
CREATE DATABASE postgress;

CREATE TABLE items (
  id SERIAL PRIMARY KEY,
  title TEXT NOT NULL
);

4️⃣ Configure Database Connection

Update your database credentials in solution.js:

const db = new Client({
  user: "postgres",
  host: "localhost",
  database: "postgress",
  password: "YOUR_PASSWORD",
  port: 5432,
});

▶️ Run the Project
nodemon index.js


Open your browser and visit:

http://localhost:3000
