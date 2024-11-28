# Node.js Testing Suite  

## Description  
This project demonstrates various aspects of testing in a Node.js application. It uses testing libraries and frameworks such as **Mocha**, **Chai**, and **Sinon** to showcase techniques like unit testing, integration testing, handling asynchronous operations, mocking, stubbing, and more.  

The project implements a simple API and utility functions that are tested using a robust test suite.  

---

## Features  
- **Task 0**: Basic testing with Mocha and the Node.js `assert` module.  
- **Task 1**: Expanding tests with support for multiple operations (`SUM`, `SUBTRACT`, `DIVIDE`).  
- **Task 2**: Transitioning to the Chai assertion library for more readable tests.  
- **Task 3**: Introduction to spies using Sinon to monitor function calls.  
- **Task 4**: Using stubs to replace and control function behavior during tests.  
- **Task 5**: Leveraging test hooks (`beforeEach` and `afterEach`) for reusable setup and cleanup.  
- **Task 6**: Writing and testing asynchronous code with callbacks.  
- **Task 7**: Skipping tests to handle incomplete or failing test cases.  
- **Task 8**: Performing basic integration testing with an Express API.  
- **Task 9**: Validating and testing routes with regular expressions.  

---

## Installation  

### Prerequisites  
- Node.js (v14 or later)  
- npm  

### Setup  
1. Clone the repository:  
   ```bash  
   git clone <repository-url>  
   ```  
2. Navigate to the project directory:  
   ```bash  
   cd nodejs-testing-suite  
   ```  
3. Install dependencies:  
   ```bash  
   npm install  
   ```  

---

## Usage  

### Running Tests  
To run the test suite, use the following command:  
```bash  
npm test  
```  

### Project Structure  
```plaintext  
.  
├── src  
│   ├── calculateNumber.js  # Utility function implementation  
│   └── app.js              # Express API setup  
├── test  
│   ├── calculateNumber.test.js  # Tests for calculateNumber  
│   ├── utils.test.js           # Tests for sendPaymentRequestToApi  
│   ├── async.test.js           # Tests for async functions  
│   ├── integration.test.js     # Integration tests for Express API  
│   └── hooks.test.js           # Tests demonstrating hooks usage  
├── package.json               # Project metadata and dependencies  
└── README.md                  # Project documentation  
```  

---

## Key Libraries and Frameworks  
- **[Mocha](https://mochajs.org/)**: A feature-rich JavaScript testing framework.  
- **[Chai](https://www.chaijs.com/)**: An assertion library for behavior-driven development.  
- **[Sinon](https://sinonjs.org/)**: A library for spies, mocks, and stubs.  
- **[Express](https://expressjs.com/)**: A minimal web framework for Node.js.  

---

## Examples  

### Example: Using Sinon Spies  
```javascript  
const sinon = require('sinon');  
const Utils = require('../src/utils');  

const spy = sinon.spy(Utils, 'calculateNumber');  
Utils.calculateNumber('SUM', 1, 2);  
console.log(spy.calledWith('SUM', 1, 2));  // Output: true  
```  

---

## Contribution  
Feel free to contribute by submitting issues or creating pull requests.  

---

## License  
This project is licensed under the MIT License.  

---  
