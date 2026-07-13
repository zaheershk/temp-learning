# Quiz CLI

> An interactive command-line quiz game for learning JavaScript and Node.js fundamentals.

## 📖 Project Overview

Quiz CLI is a terminal-based quiz application built with Node.js and ES modules. It loads categorized questions from a JSON file, prompts the player to choose a topic and question count, and then runs an interactive multiple-choice quiz with scoring, explanations, and review of incorrect answers.

This project is designed for learners who want a lightweight, dependency-free CLI experience for practicing programming concepts directly in the terminal.

## ✨ Features

- Interactive command-line quiz experience
- Category-based question selection
- Choice of all questions, 3 questions, or 5 questions when available
- Randomized question order using a Fisher-Yates shuffle
- Colorized terminal output using ANSI escape codes
- Progress indicator during the quiz
- Score summary with performance feedback
- Explanations shown after each question
- Review of incorrect answers at the end
- Replay loop so users can take the quiz again
- No external npm dependencies

## 🛠️ Tech Stack

| Layer | Technology |
|-------|------------|
| Runtime | Node.js >= 18 |
| Language | JavaScript (ES Modules) |
| CLI/Input | Built-in `node:readline` |
| File I/O | Built-in `node:fs/promises` |
| Path Handling | Built-in `node:path` and `node:url` |
| Data Format | JSON |
| Styling | ANSI escape codes |
| Package Manager | npm |

## 🗂️ Project Structure

```text
README.md                         # Project documentation

test-app/                         # Main quiz application
├── package.json                  # Project metadata and npm scripts
├── index.js                      # Application entry point
├── data/
│   └── questions.json            # Quiz questions and answer data
└── src/
    ├── colors.js                 # Terminal color helpers
    ├── input.js                  # Readline-based user input helpers
    └── quiz.js                   # Quiz logic, scoring, and results display
```

## 🚀 Setup Instructions

### Prerequisites

- Node.js 18 or newer
- npm

### Installation

The application has no external dependencies, so setup is minimal.

```bash
cd test-app
npm install
```

> `npm install` is not strictly required because the project does not declare any external packages, but running it will prepare the local `node_modules` folder if you want a standard Node.js workflow.

### Configuration

| Variable | Required | Description |
|----------|----------|-------------|
| None detected | No | No environment variables are defined in the provided codebase. |

Quiz content is stored in `test-app/data/questions.json`. To change the quiz, edit the category names, questions, answer indexes, or explanations in that file.

## 💡 Usage Examples

### Run the quiz

```bash
cd test-app
npm start
```

This launches the interactive quiz in your terminal.

### Expected flow

```text
1. Choose a category
2. Choose how many questions to answer
3. Answer multiple-choice prompts by entering a number
4. View your score and explanations
5. Choose whether to play again
```

### Run the application directly

```bash
cd test-app
node index.js
```

## 🧪 Running Tests

The package manifest defines a test script:

```bash
cd test-app
npm test
```

> ⚠️ Could not be determined from the codebase — no dedicated test files were provided in the captured repository content. If tests are added later, this command will run them via `node --test`.

## 📦 Deployment

This project is a local CLI application and does not include deployment infrastructure.

Recommended usage is to run it directly in a Node.js environment:

```bash
cd test-app
npm start
```

> ⚠️ Could not be determined from the codebase — no Dockerfile, CI/CD workflow, or hosted deployment configuration was detected.

## 🤝 Contributing

Contributions can be made by extending the question bank, improving quiz flow, or adding tests.

Suggested workflow:

1. Create a feature branch
2. Make your changes
3. Verify the quiz still runs with `npm start`
4. Add or update tests if applicable
5. Open a pull request

If you add new quiz categories or behavior, keep the JSON structure in `data/questions.json` consistent with the existing question format.

## 📄 License

This project is licensed under the MIT License.
