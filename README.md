# Beanstalk_LAB

This project demonstrates how to deploy a Node.js application using AWS Elastic Beanstalk. The application is a simple Express server that responds with a greeting message.

## Prerequisites

- AWS account
- AWS CLI installed and configured
- Node.js and npm installed

## Project Structure

- `app.js`: Main application file that sets up an Express server.
- `package.json`: Contains project metadata and dependencies.

## Getting Started

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/beanstalk_lab.git
   cd beanstalk_lab
   ```

2. **Install dependencies:**

   ```bash
   npm install
   ```

3. **Run the application locally:**

   ```bash
   npm start
   ```

   The server will start on `http://localhost:3000`.

## Deploying to AWS Elastic Beanstalk

1. **Initialize Elastic Beanstalk:**

   ```bash
   eb init
   ```

   Follow the prompts to select your AWS region and application platform (Node.js).

2. **Create an Elastic Beanstalk environment and deploy your application:**

   ```bash
   eb create beanstalk-env
   ```

3. **Open the deployed application in your default browser:**

   ```bash
   eb open
   ```

   You should see the "Hello from AWS Elastic Beanstalk!" message.

4. **Deploy updates:**

   After making changes to your application, deploy updates using:

   ```bash
   eb deploy
   ```

