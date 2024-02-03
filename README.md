# Private and Public Chat Socket.IO App

Welcome to the Private and Public Chat Socket.IO App by Lalatendu Swain!

## Introducing Private Chat Messaging with Socket.IO

![Chat App Screenshot](https://raw.githubusercontent.com/Lalatenduswain/Implementing-Private-Chat-Messaging-with-Socket.IO/master/public/img/chat-app.png "Chat")

### EXPERIENCE THE SWIFT AND ROBUST REAL-TIME ENGINE

Empowering Real-Time Chat through Socket.IO, this web application facilitates private and public conversations among multiple users. Users can engage in one-to-one chat seamlessly and efficiently. Please note that the application is coded in JavaScript ES6.

## Prerequisites

- Familiarity with [Socket.IO](https://socket.io/)
- Understanding of JavaScript ES6
- Knowledge of [WebSockets](https://developer.mozilla.org/en-US/docs/Web/API/WebSockets_API/Writing_WebSocket_client_applications)

## Installing Node.js and npm on Debian Or Ubuntu
This guide provides instructions for installing Node.js and npm on Ubuntu using the apt package manager.

### Prerequisites

- Ubuntu Or Any Debian OS operating system

### Installation

1. **Open Terminal**: Press `Ctrl+Alt+T` to open a terminal window.

2. **Update Package List**: Ensure your package list is up to date by running:

    ```bash
    sudo apt update
    ```

3. **Install Node.js and npm**: Run the following command to install Node.js and npm:

    ```bash
    sudo apt install npm nodejs -y
    ```

    The `-y` flag automatically answers yes to any prompts, making the installation non-interactive.

4. **Verify Installation**: After the installation is complete, you can verify that Node.js and npm are installed correctly by checking their versions:

    ```bash
    node -v
    npm -v
    ```

    This will display the installed versions of Node.js and npm.

### Running Locally

Ensure you have [Node.js](https://nodejs.org/) and [npm](https://www.npmjs.com/) installed.

1. Clone or Download the repository

    ```bash
    git clone https://github.com/Lalatenduswain/Implementing-Private-Chat-Messaging-with-Socket.IO.git
    cd Implementing-Private-Chat-Messaging-with-Socket.IO/
    ```

2. Install Dependencies

    ```bash
    npm install
    ```

3. Launch the application

    ```bash
    node index.js
    ```

Your app should now be accessible at [localhost:5555](http://localhost:5555/).

## Running in the Background with PM2

To ensure your Node.js application runs persistently in the background, even after you log out or close the terminal session, you can use a process manager like PM2. Follow these steps:

1. **Install PM2** (if not already installed):

    ```bash
    sudo npm install pm2@latest -g
    ```

2. **Fix npm Global Directory Permissions**:

    ```bash
    sudo chown -R $(whoami) ~/.npm
    sudo chown -R $(whoami) /usr/local/lib/node_modules
    ```

3. **Start your Node.js application with PM2**:

    ```bash
    pm2 start index.js --name chat-app
    ```

4. **Ensure the application starts automatically on server reboots**:

    ```bash
    pm2 save
    ```

5. **Check the status of your applications managed by PM2**:

    ```bash
    pm2 status
    ```

6. **Monitor your application's logs**:

    ```bash
    pm2 logs chat-app
    ```

7. **To stop the application**:

    ```bash
    pm2 stop chat-app
    ```

8. **To restart the application**:

    ```bash
    pm2 restart chat-app
    ```

9. **To remove the application from PM2**:

    ```bash
    pm2 delete chat-app
    ```

## Support or Contact

Encountering issues? Don't hesitate to submit an issue on our [GitHub page](https://github.com/Lalatenduswain/Implementing-Private-Chat-Messaging-with-Socket.IO/issues).
