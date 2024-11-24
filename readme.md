
# HW6TH_CSI3150

## 1. Problem Statement  
The Quiz app demo is a simple web-based quiz application designed to provide an engaging and interactive platform for users to test their knowledge on various topics. The app features a multiple-choice quiz format, displaying questions, tracking user responses, and providing a final score. After completing the quiz you can choose to retake or quit.

---

## 2. Functional Features of the App  
- Start Button: When 'Start' is selected the quiz directions will appear.
- Quiz Rules: Provides an overview of the quiz with options to "Continue" or to "Exit Quiz".
- Timed Questions: Each question is presented with four multiple-choice options. A 15-second timer is displayed for each question.
- Final Score Display: The app calculates and shows the users total score along with a personalized message. 

---

## 3. Codebase Overview

The app's code is modular and divided into distinct files based on functionality:

- index.html: file that is stored in the root directory to run the webpage.
- style.css: Handles the design and visual presentation of the app.
- questions.js: Stores the quiz questions and answer data.
- quizApp.js: Implements the logic for quiz functionality, including user interaction and question navigation.


---

## 4. Explanation of Relevant Files  

### **index.html**  
- Organizes content sections for instructions, the quiz interface, and the results screen.  
- Includes placeholders for dynamic content, such as questions and feedback.  

### **quizApp.js**  
- This file is responsible for bringing in all html elements and storing them as variables to be used for app functionality.
  
### **questions.js**  
- Stores questions. Example structure:  
```javascript
let questions = [
  {
    numb: 1,
    question: "What does HTML stand for?",
    answer: "Hyper Text Markup Language",
    options: [
      "Hyper Text Preprocessor",
      "Hyper Text Markup Language",
      "Hyper Text Multiple Language",
      "Hyper Tool Multi Language",
    ],
  },
```  

### **style.css**  
Responsible for the application's design:  
- Defines styles for each screen (instructions, quiz, results).  
- Includes responsive design techniques to ensure compatibility across devices.

---

## Core Functions in `quizApp.js`  

- showQuestions: This function retrieves the relevant data from the questions.js file and dynamically presents each question and its options on the screen.
- optionSelected: This function validates the selected option against the correct answer. 
- startTimerLine: Handles the display of a progress bar that visually reflects the remaining time for each question.
- queCounter: Keeps track of the current question number and updates the interface to reflect the remaining questions.
- showResult: Summarizes the quiz performance by displaying the user's final score along with a personalized message based on their results.
- startTimer: Responsible for setting up the timer for each question, managing countdown intervals, and performing actions when time expires.


---

## Styling Overview in `style.css`  

- Styling standards are applied to every aspect of the DOM. 

--- 
