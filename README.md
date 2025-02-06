📖 FAQ API
A simple and efficient FAQ Management API with Express js,MongoDB, Redis caching, and Google Translation API support. This API allows users to add, fetch, translate, and delete FAQs in multiple languages.

🚀 Features
📌 CRUD operations (Create, Read, Delete FAQs)
🌍 Multi-language support using GoogleTrans API
⚡ Redis caching for faster response times
🔐 Error handling & validation for a robust API
📦 Installation
1️⃣ Clone the Repository
git clone https://github.com/Naveenreddy7571/bharat-fd-test-full.git
2️⃣ Install Dependencies
npm install cors dotenv express googletrans ioredis mongoose redis
3️⃣ Set Up Environment Variables
Create a .env file in the root directory and add:

MONGO_URI=your_mongodb_connection_string
REDIS_PASSWORD=your_redis_password
PORT=3000
4️⃣ Start the Server
nodemon run
Your API is now running at http://localhost:3000 🎉

📌 API Endpoints
1️⃣ Add a New FAQ
POST /api/faqs
Request Body (JSON):
{
  "question": "What is this API?",
  "answer": "This is an FAQ management API."
}
Response:
{
  "message": "FAQ added successfully!"
}
2️⃣ Fetch FAQs (with Language Support)
GET /api/faqs?lang=hi
Response (Hindi translation example):
[
  {
    "question": "यह एपीआई क्या है?",
    "answer": "यह एक एफएक्यू प्रबंधन एपीआई है।"
  }
]
3️⃣ Delete an FAQ
DELETE /api/faqs/:id
Response:
{
  "message": "FAQ deleted successfully!"
}
🎯 Contribution Guidelines
Fork the repository 🍴
Clone your forked repo
git clone https://github.com/yourusername/faq-api.git
Create a new branch
git checkout -b feature-branch
Make your changes and commit 🚀
git commit -m "Added new feature"
Push your branch to GitHub 📤
git push origin feature-branch
Create a Pull Request ✅
📜 License
This project is licensed under the MIT License.

💡 Have Questions or Suggestions?
Open an issue or create a pull request. Let's make this project better together! 🚀
