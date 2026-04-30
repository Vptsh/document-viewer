# 📄 Document Viewer

A powerful and elegant **web-based document viewer** that allows users to open, preview, and interact with documents directly in the browser using URL or file upload.

---

## 🚀 Description

A sleek browser-based document viewer supporting PDF, Office, and OpenDocument formats with smart retry logic, multiple rendering providers (Google Docs, Microsoft Office), and file upload fallback via temporary hosting services.

---

## ✨ Features

### 📂 Multi-format Support
Supports a wide range of document types:
- PDF  
- DOC / DOCX  
- XLS / XLSX  
- PPT / PPTX  
- ODT / ODS / ODP  

---

### 🌐 Smart Viewer Engine
Automatically selects the best rendering provider:
- Google Docs Viewer  
- Microsoft Office Online  
- Native browser preview (fallback)  

Includes:
- Automatic retry mechanism (3 attempts)  
- Provider switching on failure  
- Timeout handling  

---

### 📤 File Upload Support
Upload files directly from your device:
- Uses **catbox.moe** (primary)  
- Fallback to **tmpfiles.org**  
- Temporary hosting (auto-expiry)  

---

### ⚡ Advanced UI/UX
- Clean iOS-inspired UI  
- Dark mode support (auto-detect)  
- Animated loader with progress tracking  
- Scroll progress indicator  
- Drag & drop upload  
- Toast notifications  

---

### 🔄 Resilient Loading System
- Multi-provider fallback  
- Smart detection of failed loads  
- Retry visualization with progress dots  
- Graceful error handling  

---

## 🖥️ How It Works

### 1. Load via URL
Paste a file link:
```
https://example.com/file.pdf
```

### 2. Upload File
- Drag & drop file  
- Or use upload button  

### 3. Viewer Resolution Logic

| Attempt | Provider |
|--------|---------|
| 1 | Google Docs Viewer |
| 2 | Microsoft Office Viewer |
| 3 | Google Drive Viewer |
| Final | Native browser |

---

## 📦 Tech Stack

- HTML5  
- CSS3 (Custom Properties, Animations)  
- Vanilla JavaScript  

---

## 📁 Project Structure

```
project/
│── index.html   # Main application file
│── README.md    # Documentation
```

---

## ⚙️ Key Components

### 🔹 Viewer Engine
Handles:
- Provider switching  
- Retry logic  
- Timeout fallback  

### 🔹 Upload System
- Catbox API integration  
- Tmpfiles fallback  
- Blob preview fallback  

### 🔹 UI System
- Loader state  
- Error state  
- Viewer state  
- Toast notifications  

---

## 🛠️ Setup & Usage

### Run Locally
```bash
git clone https://github.com/psvineet/document-viewer.git
cd document-viewer
open index.html
```

Or deploy using:
- GitHub Pages  
- Netlify  
- Vercel  

---

## 🔐 Limitations

- Uploaded files are temporary (auto-deleted after ~72 hours)  
- Cross-origin restrictions may limit preview detection  
- Some file types rely on external viewers  

---

## 📌 Future Improvements

- Add authentication-based storage  
- Improve mobile gestures (zoom/pinch)  
- Add annotation tools  
- Offline preview support  

---

## 👨‍💻 Author

Developed by **Vineet**

---

## ❤️ Acknowledgements

- Google Docs Viewer  
- Microsoft Office Online  
- Catbox.moe  
- Tmpfiles.org  

---

## 📜 License

This project is open-source and available under the MIT License.
