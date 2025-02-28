# 🏥 Healthcare Translation Web App

A **real-time, multilingual translation web app** designed to help **patients and healthcare providers** communicate effectively. The app converts **spoken input into text, provides live translation, and plays back the translated audio**. 

---

## **✨ Features**
✅ **Voice-to-Text:** Convert speech into text using the Web Speech API.  
✅ **Real-Time Translation:** Translate text into multiple languages using LibreTranslate.  
✅ **Audio Playback:** Listen to translated text with text-to-speech functionality.  
✅ **User Authentication:** Register and log in before using the translator.  
✅ **Mobile-Friendly UI:** Optimized for both desktop and mobile devices.  

---

## **🛠️ Technologies Used**
- **Frontend:** HTML, CSS, JavaScript  
- **Backend:** Python (Flask)  
- **Database:** PostgreSQL 
- **Translation API:** MyMemory  
- **Speech-to-Text API:** Web Speech API  
- **Text-to-Speech API:** Web Speech API  

---

## **🚀 Installation Guide**
1️⃣ Install Dependencies
Make sure you have **Python 3** installed. Then, install the required dependencies:  
```sh
pip install flask 
pip install flask-cors
pip install requests



📌 Running the Application
1️⃣ Start the Backend Server
In the terminal of the Backend folder:
python app.py

The Flask server will start at http://127.0.0.1:5002.

2️⃣ Open the Frontend
Open index.html in a browser.
Login/Register to access the translator.

🔹 User Authentication
Register: POST /register
json
Copy
Edit
{ "name": "John Doe", "email": "john@example.com", "password": "secure123" }
Login: POST /login
json
Copy
Edit
{ "email": "john@example.com", "password": "secure123" }
🔹 Translation
Translate Text: POST /translate
json
Copy
Edit
{ "text": "Hello", "targetLang": "es" }
Response:
json
Copy
Edit
{ "translatedText": "Hola" }
