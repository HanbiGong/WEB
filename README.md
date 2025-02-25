# 📚 Library API

Welcome to the Library API! This API allows users to browse, borrow, and return books easily.

## 🚀 Getting Started

### 📌 Prerequisites
- Node.js (v14 or higher)
- npm (Node Package Manager)

### 🛠 Installation & Setup
1. Clone this repository:
   ```bash
   git clone https://github.com/your-repo/library-api.git

2. Navigate into the project folder:
      ```bash
  cd library-api
  
3. Install dependencies:
   ```bash
  npm install
  
4.Start the server:
  node index.js
  
5.Open in the browser:
http://localhost:3000

#### 📄 API Endpoints

Method	Endpoint	Description
POST	/borrow	Borrow a book
POST	/return	Return a book
GET	/check-late	Check overdue status

##### 🎨 Customizing the Homepage

The homepage (/) is styled with CSS and includes a background image.

##### 🖼 Adding a Custom Background Image
Place your image inside the public folder and name it background.jpg.
Ensure the file path is:
/public/background.jpg
The homepage will now use your custom image as the background.

###### 🛠 Built With

Node.js - JavaScript runtime
Express.js - Web framework
Luxon - Date/time handling
Swagger - API documentation
