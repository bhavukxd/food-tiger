

# MERN App - Day 1 Setup

This guide outlines the steps to set up the frontend of a MERN stack application using React and Bootstrap.

---

## **Step 1: Create a React App**

To initialize a new React app, run the following command in your terminal:

```bash
npx create-react-app mernapp
```

### **Navigate into the Project Directory**

```bash
cd mernapp
```

---

## **Step 2: Install Bootstrap**

### **Option 1: Install via npm**

Run the following command to install Bootstrap:

```bash
npm install bootstrap
```

### Import Bootstrap CSS

After installation, import Bootstrap CSS into your `src/index.js` file:

```javascript
// src/index.js
import 'bootstrap/dist/css/bootstrap.min.css';
import React from 'react';
import ReactDOM from 'react-dom/client';
import App from './App';
import './index.css';

const root = ReactDOM.createRoot(document.getElementById('root'));
root.render(
  <React.StrictMode>
    <App />
  </React.StrictMode>
);
```

---

## **Step 3: Verify Bootstrap Integration**

### Edit `App.js`

Replace the default code in `src/App.js` with the following:

```javascript
import React from 'react';

function App() {
  return (
    <div className="container text-center mt-5">
      <h1 className="text-primary">Welcome to the MERN App</h1>
      <button className="btn btn-success">Click Me!</button>
    </div>
  );
}

export default App;
```

---

## **Step 4: Start the Application**

Run the following command to start the development server:

```bash
npm start
```

### Expected Output:

- A heading with the text **"Welcome to the MERN App"** styled in Bootstrap's primary color (blue).
- A green button styled using Bootstrap.

---



### **Day 1 Setup Complete!**
