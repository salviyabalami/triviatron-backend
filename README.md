# 🧠 Triviatron Backend

This is the backend server for **Triviatron**, a streak-based trivia game where users answer rapid-fire questions to build their longest correct answer streak.

🔗 **Frontend (Live Game):** [https://salviyabalami.github.io/triviatron](https://salviyabalami.github.io/triviatron)  
🔗 **Backend (API Endpoint):** [https://triviatron-backend.onrender.com](https://triviatron-backend.onrender.com)

---

## ⚙️ Tech Stack

- **Server:** Node.js + Express
- **Deployment:** [Render](https://render.com)
- **Data Source:** Static JSON files for questions

---

## 📁 Endpoints

### `GET /triviatron/welcome-text`
Returns a short welcome message for the game’s home screen.

### `GET /triviatron/question`
Returns a randomly selected trivia question with options (but without the answer).

### `POST /triviatron/answer`
Validates the selected answer for a given question ID.

#### Request Body:
```json
{
  "id": 3,
  "selected": "Nikola Jokic"
}
