# Cypress-startup-project
Dummy cypress project to get a start on writing cypress tests

## Setup

1. **Clone the Repository:**
- git clone [repository-url]

2. **Install Dependencies:**
- npm install
- npm install cypress
- npx cypress open

3. **Environment Variables:** - if needed
- Set the following variables in your system environment:
  - `YOUR_VARIABLE`:[variable-value]
  - `SECOND_VARIABLE`:[variable-value2]

## Setting Up Docker
Install docker desktop and open app
1. **Build Docker Image:**
docker build . -t TestSuit_Name

2. **Run Docker Container:**
docker run -e YOUR_VARIABLE="variable-value" -e SECOND_VARIABLE="variable-value2"  TestSuit_Name

## Tests description
Tests can be structured by componenets, functionalities, controllers, depending on project needs.
With this structure you can also choose wich tests to run in different situations.

Example
###  1. Tests Login Test - UI

- **Description:**
Ensure successful user login.

- **Test Command:**
cy_run:login-ui  - runs only the set of UI tests related to login

- **Expected Result:**
User should be logged in successfully.

###  1. Tests Login Test - API

- **Description:**
Ensure successful user login through API

- **Test Command:**
cy_run:login-api  - runs only the set of API tests related to login

- **Expected Result:**
User should be logged in successfully.

- **Test Result Format:**
- Pass: Green ✔️
- Fail: Red ❌

## Interpreting Failing Tests

- If a test fails:
1. Check the error message in the Cypress runner.
2. Inspect the failed step for more details.
3. Refer to the specific test code for troubleshooting.

## Additional Docker Notes

- Ensure Docker is installed and running on your machine.
- Docker commands should be executed in the root directory of the cloned repository.
