# 📬 FeedbackBox API

The **FeedbackBox API** is the backend service for the FeedbackBox application — a platform for collecting, managing, and responding to user suggestions in real time.  
Built with **Ruby on Rails**, this API provides secure authentication, suggestion management, comments, polls, notifications, and more.  
Designed to work seamlessly with the **FeedbackBox React frontend**.

---

## 🚀 Features

- **User Authentication**: Sign up, login, and secure sessions with [Devise](https://github.com/heartcombo/devise) and [OmniAuth](https://github.com/omniauth/omniauth) (Google login).
- **Suggestion Management**: Create, update, delete, and vote on suggestions.
- **Comments & Discussions**: Comment threads for each suggestion.
- **Polls**: Optional polls linked to suggestions for structured feedback.
- **Notifications**: Real-time updates using ActionCable + browser push notifications.
- **Activity Feed**: Track actions (new suggestions, votes, comments, status updates).
- **Role-based Access**: Different permissions for admins, moderators, and regular users.
- **API-Only Architecture**: Designed to be consumed by a React (or any) frontend.

---

## 🛠️ Tech Stack

- **Language**: Ruby (v3.2+ recommended)
- **Framework**: Ruby on Rails (API mode)
- **Database**: PostgreSQL
- **WebSockets**: ActionCable
- **Authentication**: Devise + OmniAuth (Google)
- **Push Notifications**: Service Workers
- **Deployment**: Render / Railway / Heroku compatible

---

## 📦 Installation

```bash
# 1️⃣ Clone the repository
git clone https://github.com/your-username/feedbackbox-api.git
cd feedbackbox-api

# 2️⃣ Install dependencies
bundle install

# 3️⃣ Set up environment variables
cp .env.example .env
# Fill in your database credentials, Google OAuth keys, and secret keys

# 4️⃣ Set up the database
rails db:create db:migrate db:seed

# 5️⃣ Start the server
rails server
