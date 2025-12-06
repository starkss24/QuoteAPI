📝 Mini Quote Saver
A lightweight web application that allows users to save, view, and delete their favorite quotes. This project focuses on data persistence using the browser's Local Storage API, ensuring quotes remain available even after the page is refreshed or the browser is closed.

🚀 Live Demo
<img width="1851" height="838" alt="image" src="https://github.com/user-attachments/assets/461a839b-210d-4984-a43d-e9e26b3192de" />


🎯 Features
Add Quotes: Input text to add new quotes to the list.

Persistent Storage: Quotes are saved instantly to localStorage. Data survives page refreshes.

Delete Quotes: Remove specific quotes from the list and storage.

Dynamic Rendering: The list updates automatically without reloading the page.

🛠️ Technologies Used
HTML5: Structure and Semantic tags.

CSS3: Styling and layout.

JavaScript (ES6+): DOM manipulation and Logic.

Web API: window.localStorage.

🧠 What I Learned
This project was built to master the concept of client-side data persistence. Key learning outcomes included:

1. The Local Storage API
I learned how to interact with the browser's storage using the setItem, getItem, and removeItem methods.

2. JSON Serialization
Since localStorage only stores strings, I learned how to convert arrays/objects to strings and back using JSON methods:

JavaScript

// Saving data
localStorage.setItem('quotes', JSON.stringify(myQuotesArray));

// Retrieving data
const storedQuotes = JSON.parse(localStorage.getItem('quotes'));
3. CRUD Operations
I implemented Create (Add), Read (Load on refresh), and Delete functionality using vanilla JavaScript arrays.

📂 Project Structure
Plaintext

/mini-quote-saver
│
├── index.html      # Main HTML structure
├── style.css       # Styles for the application
├── script.js       # Logic for localStorage and DOM manipulation
└── README.md       # Project documentation
💻 How to Run Locally
Clone the repository:

Bash

git clone https://github.com/your-username/mini-quote-saver.git
Navigate to the project directory:

Bash

cd mini-quote-saver
Open index.html in your preferred browser (or use the Live Server extension in VS Code).

🔮 Future Improvements
Add an "Edit Quote" feature.

Categorize quotes (e.g., "Motivational", "Funny").

Add a "Copy to Clipboard" button for each quote.

Made with ❤️ by Vishwak

💡 A Tip for your Code
Since you are showcasing this on GitHub, make sure your JavaScript code handles the "empty state" (when a user visits for the first time).

Inside your script.js, you likely have a line like this:

JavaScript

// Good practice: If nothing is in storage, start with an empty array []
let quotes = JSON.parse(localStorage.getItem('quotes')) || [];
