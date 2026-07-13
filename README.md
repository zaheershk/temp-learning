# Quiz CLI

An interactive command-line quiz game for learning JavaScript, Node.js, and general programming concepts.

## Overview

Quiz CLI is a simple terminal-based quiz application built with modern Node.js and ES Modules. It loads questions from a JSON file, lets users choose a category, and then walks them through a timed-free quiz experience with scoring and answer review.

## Features

- Interactive command-line interface
- Multiple quiz categories
- Randomized question order
- Score tracking and final results summary
- Answer explanations for learning
- Built with native Node.js modules only

## Tech Stack

- Node.js 18+
- JavaScript (ES Modules)
- Built-in `readline` module for terminal input
- Built-in `fs/promises` for loading quiz data

## Project Structure

```text
quiz-cli/
└── test-app/
    ├── data/
    │   └── questions.json
    ├── index.js
    ├── package.json
    └── src/
        ├── colors.js
        ├── input.js
        └── quiz.js
```

## Setup

1. Install Node.js 18 or newer.
2. Clone the repository.
3. Navigate to the application directory:

```bash
cd test-app
```

4. Install dependencies:

```bash
npm install
```

> The project currently uses only built-in Node.js modules, so no external packages are required.

## Usage

Run the quiz application with:

```bash
npm start
```

You will be prompted to:

1. Choose a quiz category
2. Select how many questions to answer
3. Respond to each question from the terminal
4. Review your score and incorrect answers at the end

## Tests

A test script is available in `package.json`:

```bash
npm test
```

At the moment, the project does not include automated test files, so this command may need future test coverage to be added.

## Deployment

This application is designed to run locally in a terminal environment. To share or deploy it:

- Publish the repository to GitHub
- Ensure the target environment has Node.js 18+
- Run the app from the `test-app` directory using `npm start`

## Contributing

Contributions are welcome. A simple workflow is:

1. Create a feature branch
2. Make your changes
3. Test the application manually
4. Open a pull request with a clear description of your changes

## License

This project is licensed under the MIT License.
