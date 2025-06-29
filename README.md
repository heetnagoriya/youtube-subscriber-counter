# 📊 YouTube Subscriber Counter

A sleek and modern real-time web application to fetch and display **live subscriber counts** for any YouTube channel using just a username, handle, or channel ID.

## 🖼️ Live Demo

🚀 **[Click here to use the app →](http://youtube-subscriber-site-heet.s3-website.ap-south-1.amazonaws.com/)**  
*(Best viewed on desktop)*

---

## ⚙️ Tech Stack

| Frontend     | Backend      | APIs              | Hosting       |
|--------------|--------------|-------------------|----------------|
| HTML, CSS, JS| AWS Lambda   | YouTube Data API  | AWS S3 (Static Website) |
| Responsive UI| API Gateway  |                   |                |

---

## ✨ Features

✅ Real-time subscriber count for any public YouTube channel  
✅ Input support for: Any Youtube Channel Name/URL/ Channel I'D


✅ Auto-refresh every 30 seconds  
✅ Mobile-responsive & modern gradient UI  
✅ Spinner & error messages with graceful UX handling

---

## 📁 Project Structure

youtube-subscriber-counter/
│
├── index.html # Fully responsive frontend UI
├── lambda/
│ └── lambda_function.py # AWS Lambda backend logic
└── README.md # This file

## 🧠 How It Works

1. User enters a YouTube handle/username/ID in the form.
2. JavaScript sends a `GET` request to an **AWS API Gateway endpoint**.
3. That endpoint triggers a **Lambda function** which:
   - Parses the username
   - Requests subscriber data from **YouTube Data API v3**
   - Sends back the response (channel name, subscribers, thumbnail, etc.)
4. Frontend displays it beautifully — live & auto-refreshing.

---

## 🔐 API Notes

- The backend uses the **YouTube Data API v3**, which requires an API Key.
- It handles:
  - Channel by Username
  - Channel by ID
  - Channel by Custom Handle (starts with `@`)
- Error-handled responses for invalid inputs or API failures.

---

## 🧑‍💻 Author

**Heet N.**  
🔗 [GitHub Profile](https://github.com/heetnagoriya)  
📧 [Email](heetnagoriya@gmail.com) 
💼 Passionate about Backend Engineering, AWS, and building full-stack solutions.

---

## 💡 Future Improvements (Optional)

- Add search history with local storage
- Support dark/light theme switch
- Deploy backend as container (for cold start optimization)
- Add charts showing subscriber growth

---

## 🙌 Support

If you liked this project, please ⭐️ the repository to support it!
