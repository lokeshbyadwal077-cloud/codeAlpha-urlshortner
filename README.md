CodeAlpha project

url shortner

🔗 CodeAlpha URL Shortener

A simple and responsive URL Shortener built using Node.js, Express.js, and MongoDB. This application converts long URLs into short, shareable links and redirects users to the original website using the generated short URL.
____________________________________________________________________________________________________________________________________________________
🚀 Features

✅ Shorten long URLs 

✅ Generate unique short codes

✅ Custom alias support

✅ URL validation

✅ Redirect to original URL

✅ Store URLs in MongoDB

✅ Click tracking

✅ QR Code generation

✅ Copy shortened URL

✅ Delete shortened URLs

✅ Responsive user interface
____________________________________________________________________________________________________________________________________________________
🛠️ Tech Stack

Frontend: HTML, CSS, JavaScript
Backend: Node.js, Express.js
Database: MongoDB (Mongoose)
Packages: nanoid, valid-url, dotenv, cors
____________________________________________________________________________________________________________________________________________________
📁 Project Structure

CodeAlpha_URLShortener/
│
├── config/
│   └── db.js
├── controllers/
│   └── urlController.js
├── models/
│   └── Url.js
├── routes/
│   └── urlRoutes.js
├── public/
│   ├── index.html
│   ├── style.css
│   ├── script.js
│   └── 404.html
├── .env
├── .gitignore
├── package.json
├── server.js
└── README.md

____________________________________________________________________________________________________________________________________________________
⚙️ Installation

1. Clone the Repository
git clone https://github.com/lokeshbyadwal077/CodeAlpha_URLShortener.git
2. Navigate to Project
cd CodeAlpha_URLShortener
3. Install Dependencies
npm install
4. Create a .env File
PORT=5000
MONGO_URI=your_mongodb_connection_string
BASE_URL=http://localhost:5000
5. Start the Server
npm start
For development:

npm run dev
____________________________________________________________________________________________________________________________________________________
📌 API Endpoints

Shorten URL
POST /api/shorten

Request

{
  "originalUrl": "https://www.google.com"
}
Response

{
  "success": true,
  "data": {
    "shortUrl": "http://localhost:5000/abc123"
  }
}
____________________________________________________________________________________________________________________________________________________
Redirect

GET /:shortCode
Example

http://localhost:5000/abc123
Automatically redirects to the original URL.
____________________________________________________________________________________________________________________________________________________
Get URL Statistics

GET /api/stats/:shortCode
____________________________________________________________________________________________________________________________________________________
Delete URL

DELETE /api/url/:shortCode
____________________________________________________________________________________________________________________________________________________
📸 Screenshots

Add screenshots of:

Home Page
URL Shortened Successfully
QR Code
MongoDB Collection
Redirect Working
____________________________________________________________________________________________________________________________________________________
🔮 Future Improvements

User Authentication
Custom Dashboard
URL Analytics
URL Expiration Notifications
Password Protected URLs
____________________________________________________________________________________________________________________________________________________
👨‍💻 Author

Lokesh Meena

🎓 BCA Student
💻 Full Stack Web Developer
🌱 Learning Java, Node.js
GitHub: https://github.com/in/Lokesh-Meena007
LinkedIn:www.linkedin.com/in/lokesh-meena-1b4a09383
____________________________________________________________________________________________________________________________________________________
📄 License

This project was developed as part of the CodeAlpha Internship Program for educational and learning purposes.
