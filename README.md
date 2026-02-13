# 🎯 Dynamic Event Management System

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

> A modern, interactive event management application demonstrating advanced DOM manipulation techniques and dynamic content generation.

## 📋 Project Information

- **Student Name:** Yagyansh Singh Ahlawat
- **Roll Number:** 2501010120
- **University:** K.R. Mangalam University
- **Subject:** Web Development-2
- **Faculty:** Mr. Devendra Kumar Gupta
- **Assignment:** Assignment 1 - DOM Manipulation & Event Handling

---

## 🌟 Features

### Core Functionality
- ✨ **Dynamic Event Creation** - Add events with title, date, category, and description
- 🗑️ **Individual Event Deletion** - Remove specific events with a single click
- 🧹 **Bulk Actions** - Clear all events at once
- 📝 **Sample Data Generation** - Quickly populate with example events
- ⌨️ **Keyboard Event Detection** - Real-time keypress display

### DOM Manipulation Demonstrations
- 📚 **Educational Section** - Interactive comparison of:
  - `innerHTML` - Renders HTML tags
  - `innerText` - Removes HTML, collapses whitespace
  - `textContent` - Removes HTML, preserves whitespace

### Technical Highlights
- 🎨 Modern gradient-based UI design
- 📱 Fully responsive layout using CSS Grid
- 🔄 Real-time DOM updates without page reload
- 🎭 Smooth animations and hover effects
- 💜 Clean, professional purple-blue color scheme

---

## 🚀 Technologies Used

| Technology | Purpose |
|------------|---------|
| **HTML5** | Semantic structure and form elements |
| **CSS3** | Styling, Grid layout, gradients, animations |
| **Vanilla JavaScript** | DOM manipulation, event handling, dynamic content |

---

## 📸 Screenshots

### Main Interface
The application features a two-column layout with an event creation form on the left and event display area on the right.

### Key Components
1. **Event Form** - Input fields for event details
2. **Event Cards** - Dynamically generated event displays
3. **DOM Demo Section** - Educational content about DOM properties
4. **Interactive Controls** - Clear all and sample data buttons

---

## 🛠️ Installation & Setup

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- A text editor (VS Code, Sublime Text, etc.)
- Basic understanding of HTML, CSS, and JavaScript

### Steps to Run

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd event-management-system
   ```

2. **Open the project**
   - Simply open `index.html` in your web browser
   - Or use a local server (recommended):
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js (with http-server)
   npx http-server
   ```

3. **Access the application**
   - Direct: Open `index.html` in browser
   - Server: Navigate to `http://localhost:8000`

---

## 💻 Code Structure

```
event-management-system/
│
├── index.html          # Main HTML structure
├── style.css           # Styling and layout
├── script.js           # JavaScript logic and DOM manipulation
└── README.md           # Documentation
```

### File Descriptions

#### `index.html`
- Semantic HTML5 structure
- Event creation form with validation-ready inputs
- Event display container
- DOM manipulation demonstration section
- Keyboard event listener display

#### `style.css`
- CSS Grid layout for responsive design
- Gradient backgrounds and modern aesthetics
- Smooth hover effects and transitions
- Mobile-friendly styling
- Component-based class naming

#### `script.js`
- Form submission event handler
- Dynamic card creation using `createElement()`
- Event delegation for delete functionality
- Keyboard event detection
- Sample data generation

---

## 🎓 Learning Outcomes

This project demonstrates proficiency in:

1. **DOM Manipulation**
   - Creating elements dynamically (`createElement`)
   - Adding/removing elements (`appendChild`, `remove`)
   - Modifying element content (`innerHTML`, `textContent`)
   - Class manipulation (`classList.add`)

2. **Event Handling**
   - Form submission events
   - Click events with event delegation
   - Keyboard events (`keydown`)
   - Preventing default behaviors (`preventDefault`)

3. **Modern CSS Techniques**
   - CSS Grid layout
   - Linear gradients
   - Flexbox for card layouts
   - Pseudo-classes and hover effects
   - Box shadows and border radius

4. **JavaScript Best Practices**
   - Query selectors for DOM access
   - Event listeners for interactivity
   - Template literals for HTML generation
   - Functional programming concepts

---

## 🔍 Key Concepts Demonstrated

### 1. Event Object
```javascript
form.addEventListener('submit', (e) => {
    e.preventDefault(); // Prevent form submission
    // Process form data
});
```

### 2. Dynamic Content Creation
```javascript
const card = document.createElement('div');
card.classList.add('card');
card.innerHTML = `<h3>${title}</h3>...`;
eventcards.appendChild(card);
```

### 3. Event Delegation
```javascript
const dlt = card.querySelector('.dlt');
dlt.addEventListener('click', () => {
    card.remove();
});
```

### 4. Keyboard Events
```javascript
document.addEventListener('keydown', (event) => {
    output.textContent = "You pressed: " + event.key;
});
```

---

## 📊 Features Breakdown

### Event Categories
- 🎤 Conference
- 🛠️ Workshop
- 👥 Meetup
- 💻 Webinar
- 🎉 Social

### User Actions
- ➕ Add new events via form
- ❌ Delete individual events
- 🗑️ Clear all events
- 📋 Add sample events for testing
- ⌨️ Track keyboard input

---

## 🎨 Design Principles

- **Clean Interface** - Minimalist design focusing on functionality
- **Visual Hierarchy** - Clear distinction between form and content areas
- **Color Psychology** - Calming purple-blue palette for productivity
- **Accessibility** - Readable fonts and good contrast ratios
- **Responsiveness** - Adapts to different screen sizes

---

## 🐛 Known Issues & Future Enhancements

### Current Limitations
- Sample button creates two events instead of one (duplicate event listener)
- No data persistence (events clear on page reload)
- No form validation for empty fields

### Potential Improvements
- [ ] Add localStorage for data persistence
- [ ] Implement form validation
- [ ] Add edit functionality for existing events
- [ ] Include event search/filter feature
- [ ] Add event sorting by date or category
- [ ] Implement drag-and-drop reordering
- [ ] Export events to calendar format
- [ ] Add event reminder notifications

---

## 📱 Browser Compatibility

| Browser | Version | Status |
|---------|---------|--------|
| Chrome | 90+ | ✅ Fully Supported |
| Firefox | 88+ | ✅ Fully Supported |
| Safari | 14+ | ✅ Fully Supported |
| Edge | 90+ | ✅ Fully Supported |

---

## 🤝 Contributing

This is an academic project, but suggestions are welcome:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Commit changes (`git commit -m 'Add improvement'`)
4. Push to branch (`git push origin feature/improvement`)
5. Open a Pull Request

---

## 📝 Assignment Criteria Met

✅ DOM manipulation techniques  
✅ Event handling (submit, click, keydown)  
✅ Dynamic content generation  
✅ CSS styling and layout  
✅ Code organization and structure  
✅ User interaction and feedback  
✅ Documentation and comments  

---

## 📞 Contact

**Yagyansh Singh Ahlawat**  
- Roll Number: 2501010120
- University: K.R. Mangalam University
- Course: Web Development-2

**Faculty Supervisor**  
Mr. Devendra Kumar Gupta

---

## 📄 License

This project is created for educational purposes as part of the Web Development-2 course curriculum at K.R. Mangalam University.

---

## 🙏 Acknowledgments

- K.R. Mangalam University for providing the learning opportunity
- Mr. Devendra Kumar Gupta for guidance and course instruction
- MDN Web Docs for JavaScript and DOM API references

---

<div align="center">

**⭐ If you find this project helpful, please consider giving it a star!**

Made with 💜 by Yagyansh Singh Ahlawat

</div>
