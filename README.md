# TCS Verbal Ability Mock Test

A web-based **TCS Verbal Ability Mock Test Platform** designed to simulate the actual exam experience with timed sections, automatic progression, typed answers, passage recall, and email writing.

## 🚀 Features

* No login or registration required
* Directly start the mock test
* TCS-style Verbal Ability sections
* Individual timer for each question/section
* Automatic progression when time expires
* Sentence Completion with **one-word typed answers**
* Passage Recall with separate reading and writing phases
* Email Writing with a realistic exam-style situation
* Automatic answer submission when time expires
* Responsive and clean exam interface
* JSON-based question bank
* Multiple accepted answers/synonyms for Sentence Completion
* Results available after completing the test

## 📝 Test Structure

| Section             | Questions |             Time |
| ------------------- | --------: | ---------------: |
| Sentence Completion |        20 |  25 sec/question |
| Instruction         |         1 |           25 sec |
| Passage Recall      |       4+4 | 120 sec/question |
| Instruction         |         1 |           15 sec |
| Email Writing       |         1 |          540 sec |

### 1. Sentence Completion

* 20 questions
* 25 seconds per question
* No multiple-choice options
* Candidate must type **one word**
* Multiple valid answers/synonyms can be configured in the question bank
* Answer is automatically submitted when the timer reaches zero

### 2. Passage Recall

The candidate is shown a passage for a limited reading period.

* **30 seconds:** Read and memorize the passage
* Passage disappears after 30 seconds
* **90 seconds:** Rewrite the passage from memory
* Total: **120 seconds**

This section is designed to simulate the memory and comprehension requirements of the TCS-style assessment.

### 3. Email Writing

* 1 email-writing question
* 540 seconds
* Candidate receives a situation/instruction
* Candidate writes a professional email based on the given situation

## 🛠️ Tech Stack

The project intentionally uses a **minimal technology stack**.

* **Frontend:** React
* **Language:** JavaScript
* **Styling:** CSS
* **Database:** JSON files
* **Build Tool:** Vite
* **Deployment:** Suitable for platforms such as Netlify or Vercel

No external database such as PostgreSQL or MongoDB is required.

## 📁 Project Structure

```text
tcs-verbal-ability-mock-test/
│
├── public/
│   └── ...
│
├── src/
│   ├── components/
│   │   ├── Timer
│   │   ├── Question
│   │   ├── Instructions
│   │   └── ...
│   │
│   ├── data/
│   │   └── questions.json
│   │
│   ├── pages/
│   │   ├── Home
│   │   ├── Test
│   │   └── Result
│   │
│   ├── App.jsx
│   └── main.jsx
│
├── package.json
├── vite.config.js
└── README.md
```

> The exact folder structure may vary depending on the current implementation.

## 📚 Question Bank

Questions are stored in JSON format, making the project simple to maintain and easy to expand.

Example:

```json
{
  "id": 1,
  "type": "sentence-completion",
  "question": "He was ___ to accept the offer.",
  "answers": [
    "reluctant",
    "unwilling",
    "hesitant"
  ]
}
```

The `answers` array allows the application to accept multiple valid synonyms where appropriate.

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/your-username/tcs-verbal-ability-mock-test.git
```

Navigate to the project directory:

```bash
cd tcs-verbal-ability-mock-test
```

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

Open the local URL displayed by Vite in your browser.

## 🏗️ Build for Production

```bash
npm run build
```

To preview the production build:

```bash
npm run preview
```

## 🎯 Project Objective

The main objective of this project is to provide students preparing for **TCS recruitment examinations** with a realistic and easily accessible environment for practicing Verbal Ability.

Instead of using a traditional quiz format, the application focuses on **exam simulation**, including:

* Strict time limits
* Automatic section progression
* Typed responses
* Memory-based passage recall
* Professional email writing
* Minimal distractions during the test

## 🔮 Future Improvements

Possible future enhancements include:

* 500+ question question-bank
* Randomized questions
* Multiple mock-test sets
* Detailed performance analysis
* Accuracy and time analysis
* Difficulty-based questions
* Leaderboard
* Dark mode
* Mobile optimization
* Admin panel for managing questions
* More TCS NQT sections such as Numerical Ability and Reasoning Ability

## ⚠️ Disclaimer

This is an **independent practice project** created for educational purposes.

It is not affiliated with, endorsed by, or officially connected to **Tata Consultancy Services (TCS)**.

The questions and test format are intended to provide a practice experience based on publicly available information and commonly reported TCS-style assessment patterns.

## 👨‍💻 Author

**Shishir Mishra**

MCA Student | Web Developer | Competitive Programming & Placement Preparation

---

⭐ If you find this project useful, consider giving the repository a **star** on GitHub.
