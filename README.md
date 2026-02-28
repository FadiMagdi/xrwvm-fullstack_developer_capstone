# xrwvm-fullstack_developer_capstone
# fullstack_developer_capstone

> Your ultimate destination for finding the best car dealerships and reading real customer reviews.

---

## 📖 About

**Best Cars** is a web platform that helps car buyers make informed decisions by providing access to a wide network of car dealerships along with genuine customer reviews. Whether you're looking for a new ride or just researching your options, Best Cars gives you everything you need in one place.

---

## ✨ Features

- **Browse Dealerships** — Explore a wide list of car dealerships across multiple locations
- **Read Reviews** — View honest, real customer reviews for each dealership
- **Sentiment Analysis** — Reviews are tagged as positive, neutral, or negative so you can quickly gauge dealership quality
- **User Accounts** — Register and log in to post your own reviews and manage your profile
- **Search & Filter** — Find dealerships by name, location, or state
- **Post a Review** — Share your experience with a dealership to help other buyers

---

## 🛠️ Tech Stack

| Layer      | Technology            |
|------------|-----------------------|
| Frontend   | React.js              |
| Backend    | Django (Python)       |
| Database   | SQLite / PostgreSQL   |
| Deployment | Kubernetes (IBM Cloud)|
| CI/CD      | GitHub Actions        |

---

## 🚀 Getting Started

### Prerequisites
- Python 3.11+
- Node.js 14+
- pip & npm

### Installation

1. **Clone the repository**
```bash
   git clone https://github.com/your-username/best-cars.git
   cd best-cars
```

2. **Set up the backend**
```bash
   cd server
   pip install -r requirements.txt
   python manage.py makemigrations
   python manage.py migrate
   python manage.py runserver
```

3. **Set up the frontend**
```bash
   cd server/frontend
   npm install
   npm run build
```

4. **Visit the app**
```
   http://localhost:8000
```

---

## 📁 Project Structure
```
best-cars/
├── server/
│   ├── djangoapp/          # Main Django application
│   ├── djangoproj/         # Django project settings
│   ├── frontend/           # React frontend
│   │   └── src/
│   │       ├── components/ # React components
│   │       └── assets/     # Images and styles
│   └── manage.py
├── .github/
│   └── workflows/
│       └── main.yml        # CI/CD workflow
├── Dockerfile
├── deployment.yaml
└── README.md
```

---

## 🔁 CI/CD

This project uses **GitHub Actions** to automatically lint Python and JavaScript files on every push or pull request to the `main` branch.

---

## 🌐 Deployment
```bash
docker build -t us.icr.io/$MY_NAMESPACE/dealership .
docker push us.icr.io/$MY_NAMESPACE/dealership
kubectl apply -f deployment.yaml
```

---

## 🤝 Contributing

1. Fork the repository
2. Create a branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

---

## 📄 License

MIT License — see [LICENSE](LICENSE) for details.

---

## 👤 Author

Made with ❤️ by **Fadi Magdi**
