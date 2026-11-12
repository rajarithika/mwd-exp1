#  Exp1 –  React Lab Exercise: Understanding React File Structure

## **NAME: Raja Rithika**

## **REG NO: 2305001029**

---

## Aim

To create a basic React application using Vite and understand the purpose of important files and folders in the React project structure.

## Objectives

- Create a React project using Vite.
- Identify important React files and folders.
- Understand the role of `main.jsx`, `App.jsx`, `index.html`, and `package.json`.
- Create and use simple React components.
- Run and test a React application.

## Program

### Step 1: Create a React Project

Execute the following commands in the VS Code terminal:

```bash
npm create vite@latest student-app
cd student-app
npm install
npm run dev
```

Select React as the framework and JavaScript as the variant.

### Step 2: Understand the File Structure

```text
student-app/
│
├── node_modules/
├── public/
├── src/
│   ├── assets/
│   ├── components/
│   │   ├── Student.jsx
│   │   ├── Course.jsx
│   │   └── Faculty.jsx
│   │
│   ├── App.css
│   ├── App.jsx
│   ├── index.css
│   └── main.jsx
│
├── index.html
├── package.json
├── package-lock.json
└── vite.config.js
```

### Step 3: Understand index.html

The `index.html` file contains the root element where the React application is displayed.

```html
<div id="root"></div>
```

### Step 4: Understand main.jsx

The `main.jsx` file is the entry point of the React application. It connects React with the HTML root element and renders the App component.

### Step 5: Create App.jsx

Open `src/App.jsx` and add the following code:

```jsx
import './App.css'
import Student from './components/Student'
import Course from './components/Course'
import Faculty from './components/Faculty'

function App() {
  return (
    <div className="container">
      <h1>Student Information System</h1>

      <Student />
      <Course />
      <Faculty />
    </div>
  )
}

export default App
```

### Step 6: Create Student.jsx

Create a `components` folder inside `src` and add `Student.jsx`.

```jsx
import '../App.css'

function Student() {
  return (
    <div className="student">
      <h2>Student Details</h2>

      <p>Name: Raja Rithika</p>
      <p>Register Number: 2305001029</p>
      <p>Department: CSE</p>
    </div>
  )
}

export default Student
```

### Step 7: Create Course.jsx

Create `Course.jsx` inside the components folder.

```jsx
import '../App.css'

function Course() {
  return (
    <div className="student">
      <h2>Course Details</h2>

      <p>Course: AI1067 - Modern Web Application Development</p>
      <p>Semester: VII</p>
      <p>Credits: 3</p>
    </div>
  )
}

export default Course
```

### Step 8: Create Faculty.jsx

Create `Faculty.jsx` inside the components folder.

```jsx
import '../App.css'

function Faculty() {
  return (
    <div className="student">
      <h2>Faculty Details</h2>

      <p>Name: Ajith Kumar</p>
      <p>Department: CSE</p>
      <p>Designation: Professor</p>
      <p>College: Saveetha Engineering College</p>
    </div>
  )
}

export default Faculty
```

### Step 9: Import Components in App.jsx

Import all three components into the main App.jsx file.

```jsx
import './App.css'
import Student from './components/Student'
import Course from './components/Course'
import Faculty from './components/Faculty'

function App() {
  return (
    <div className="container">
      <h1>Student Information System</h1>

      <Student />
      <Course />
      <Faculty />
    </div>
  )
}

export default App
```

### Step 10: Add CSS in App.css

Open `src/App.css` and add:

```css
.container {
  text-align: center;
  padding: 30px;
}

.student {
  border: 1px solid #ccc;
  padding: 20px;
  margin: 20px auto;
  width: 300px;
}

.student h2 {
  color: blue;
}

.student p {
  color: green;
}
```

## Output

**Student Information System**
<img width="1600" height="899" alt="WhatsApp Image 2026-11-11 at 12 52 00 AM" src="https://github.com/user-attachments/assets/bd980b45-9482-469c-b5b3-74b06ec0281e" />


## Result

Thus, a basic React application was successfully created using Vite. The React file structure was understood, and reusable components were created and displayed successfully.
