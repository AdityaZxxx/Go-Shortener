# **URL Shortener - Go Backend**

A simple yet powerful URL shortener service built with **Go (Golang)** backend and modern web frontend. Create short links quickly or customize your own short URLs.

![URL Shortener Screenshot](/screenshot.png)

## **✨ Features**

- **Shorten URLs** instantly with auto-generated keys
- **Custom short URLs** (e.g., `yourdomain.com/mylink`)
- **Copy to clipboard** button for easy sharing
- **Responsive design** works on mobile & desktop
- **Dark/Light mode** toggle
- **Simple API** for integrations

## **🚀 Quick Start**

### **Prerequisites**

- Go 1.20+
- Git

### **Run Locally**

1. Clone the repo:

   ```bash
   git clone https://github.com/AdityaZxxx/GO-Shortener.git
   cd url-shortener
   ```

2. Run the server:

   ```bash
   go run main.go
   ```

3. Open in browser:
   ```
   http://localhost:8080
   ```

## **🛠️ Deployment**

### **Option 1: Railway (Recommended for Go)**

[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/new/template?template=https://github.com/AdityaZxxx/url-shortener)

### **Option 2: Vercel (Frontend Only)**

- Deploy the `static` and `templates` folders as a static site.

### **Option 3: Docker**

```bash
docker build -t url-shortener .
docker run -p 8080:8080 url-shortener
```

## **📂 Project Structure**

```
.
├── main.go            # Backend server
├── templates/         # HTML templates
│   └── index.html
├── static/            # CSS & assets
│   └── style.css
├── go.mod             # Go dependencies
└── README.md
```

## **🔧 API Endpoints**

| Endpoint   | Method | Description                        |
| ---------- | ------ | ---------------------------------- |
| `/shorten` | POST   | Shorten a URL (returns random key) |
| `/custom`  | POST   | Create custom short URL            |
| `/{key}`   | GET    | Redirect to original URL           |

**Example Request:**

```bash
curl -X POST -d "url=https://example.com" http://localhost:8080/shorten
```

## **🌍 Environment Variables**

| Variable | Default | Description |
| -------- | ------- | ----------- |
| `PORT`   | `8080`  | Server port |

## **🤝 Contributing**

Pull requests welcome! For major changes, open an issue first.

## **📜 License**

MIT © [Aditya Rahmad](https://github.com/AdityaZxxx)
