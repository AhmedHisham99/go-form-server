# Go Form Server

A minimal Go web application that serves a static HTML form and handles form submissions using Go’s built-in `net/http` package. This project is intentionally simple and beginner-friendly, while following clean structure and best practices.

---

## 📸 Screenshots

![Form Page](images/form-page.png)
![Form Submission Result](images/form-result.png)

---

## 🚀 Features

* Static file serving using `http.FileServer`
* HTML form with POST submission
* Server-side form parsing
* Clean and minimal project structure
* Zero external dependencies

---

## 🗂 Project Structure

```text
go-form-server/
├── main.go
├── go.mod
├── static/
│   └── form.html
├── images/
│   ├── form-page.png        
│   └── form-result.png
└── README.md
```

---

## ⚙️ How It Works

1. The server runs on port **8080**
2. Static files are served from the `static/` directory
3. The HTML form sends a `POST` request to `/form`
4. The Go handler parses and prints submitted values

---

## ▶️ Getting Started

### Prerequisites

* Go **1.20+** installed

### Run Locally

```bash
go run main.go
```

Open your browser:

```text
http://localhost:8080/form.html
```

---

## 📡 Endpoints

| Method | Path     | Description             |
| ------ | -------- | ----------------------- |
| GET    | `/`      | Static file server      |
| POST   | `/form`  | Handles form submission |
| GET    | `/hello` | Test endpoint           |

---

## 🧪 Example Output

```text
Post request successful
Name = John Doe
Address = Berlin
```

---

## 🛠 Tech Stack

* **Go** — `net/http`
* **HTML5** — form handling

---

## 📈 Future Improvements

* Add CSS styling
* Add client-side validation
* Return JSON responses
* Add Docker support
* Add unit tests

---
