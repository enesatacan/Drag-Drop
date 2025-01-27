### Daily JavaScript App - Day 29: Drag & Drop Application 🎯  

This simple and effective **Drag & Drop** application allows users to move items from one area to another using drag-and-drop functionality. Developed as part of the **Daily JavaScript Coding Challenge**, this project offers an interactive interface based on modern web technologies.

---

### ✨ Features  
- **Dynamic Drag and Drop Functionality**  
  Drag and drop items between the two boxes seamlessly.  
- **Fast and User-Friendly Interface**  
  Optimized for both desktop and mobile devices.  
- **Interactive Event Handling**  
  JavaScript powers dynamic event handling, such as `dragstart`, `dragover`, and `drop`.

---

### 📂 File Structure  
```
├── index.html          # Main HTML file  
├── style.css           # CSS file for styling  
└── script.js           # JavaScript file for dynamic functionality  
```

---

### 📋 Technologies Used  
- **HTML5**: For creating the structure of the application.  
- **CSS3**: For styling and designing an engaging layout.  
- **JavaScript**: To implement the drag-and-drop functionality dynamically.

---

### 🚀 How It Works  
1. Select an item to drag.  
2. Drag and drop it into the left or right box.  
3. The item dynamically moves to the target container.

---

### 🔧 How to Use  
1. Download or clone the project files to your local machine:  
   ```bash
   git clone https://github.com/enesatacan/Drag-Drop  
   ```  
2. Open the `index.html` file in any modern browser.  
3. Drag and drop items between the containers to test the functionality.

---

### 💻 Code Highlights  

**HTML**  
A clean and simple layout:  
```html
<div class="container">
  <div id="left">
    <div class="list" draggable="true">List Item 1</div>
    <div class="list" draggable="true">List Item 2</div>
    <div class="list" draggable="true">List Item 3</div>
  </div>
  <div id="right"></div>
</div>
```

**JavaScript**  
Dynamic event handling to enable drag-and-drop:  
```javascript
for (list of lists) {
  list.addEventListener("dragstart", function (e) {
    let selected = e.target;
    rightBox.addEventListener("drop", function () {
      rightBox.appendChild(selected);
    });
    leftBox.addEventListener("drop", function () {
      leftBox.appendChild(selected);
    });
  });
}
```

---

### Screenshot

![image](https://github.com/user-attachments/assets/f4eb9798-abc9-4216-ae76-7d0939ebe1ed)
