# Coding Quiz Application

## Overview

The Coding Quiz Application is a web-based quiz platform built with React. It allows users to take quizzes on various topics and track their scores. The application is designed to be interactive and user-friendly, providing a seamless experience for quiz takers.

## Features

- Start a quiz with a single click
- Display questions and multiple-choice answers
- Track and display the user's score
- Navigate through questions
- Submit answers and receive feedback

## Technologies Used

- **Frontend**: React, TypeScript
- **Backend**: Node.js, Express
- **Testing**: Cypress, Vitest

## Installation

To set up the application locally, follow these steps:

1. Clone the repository:
    ```sh
    git clone https://github.com:whoenig44/Testing-Tech-Suite.git
    cd Testing-Tech-Suite
    ```

2. Install dependencies:
    ```sh
    npm install
    ```
3. Build the application:
    ```sh
    npm run build
    ```

4. Seed the Database:
    ```sh
    npm run seed
    ```

5. Start the development server:
    ```sh
    npm run start:dev
    ```

4. Open your browser and navigate to `http://localhost:3001` to view the application.

## Testing

The application uses Cypress for end-to-end testing and Vitest for unit testing. Cypress tests are located in the cypress directory, and Vitest tests are located in the `tests` directory.

### Running Cypress Tests

To run Cypress tests, follow these steps:

1. Open Cypress Test Runner:
    ```sh
    npx cypress open
    ```

2. In the Cypress Test Runner window, click on the test file you want to run (e.g., [Quiz.cy.tsx]).

3. Cypress will execute the tests and display the results.

### Cypress Test Example

Here is an example of a Cypress test for the Quiz component:

```typescript
// filepath: /C:/Users/SoPro/bootcamp/homework/bootcamp-hw-19/Testing-Tech-Suite/cypress/component/Quiz.cy.tsx
import React from 'react';
import Quiz from '../../client/src/components/Quiz';

describe('<Quiz />', () => {
  it('renders', () => {
    // see: https://on.cypress.io/mounting-react
    cy.mount(<Quiz />);
  });
});
