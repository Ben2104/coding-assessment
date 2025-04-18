# Local Development with the Firebase Emulator Suite
## Prerequisites
- A simple editor such as Visual Studio Code, Atom, or Sublime Text
- Node.js 10.0.0 or higher (to install Node.js, use nvm, to check your version, run node --version) (Node.js 16.20.2 is recommended for this project)
### 🖥 If you're on macOS or Linux:
### 1. ✅ Make sure nvm is installed:
```
  nvm --version
```

If not installed, run:
```
  curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
```
Then restart your terminal or run:
```
source ~/.nvm/nvm.sh
```
### 2. 🚀 Install Node v16:
```
  nvm install 16
```
This will download and install the latest version of Node 16 (e.g. 16.20.2).

### 3. 🔄 Use Node v16:
```
  nvm use 16
```
Set it as your default if you want:
```
  nvm alias default 16
```
### 🪟 If you're on Windows:
Use nvm for Windows (it’s a separate tool):

### 1. Download from:
https://github.com/coreybutler/nvm-windows/releases

Install it like a regular Windows program.

### 2. Install Node v16:
Open Command Prompt or PowerShell:
```
  nvm install 16
  nvm use 16
```
✅ Verify it works:
```
  node -v
  npm -v
```
- Java 7 or higher (to install Java use these instructions, to check your version, run java -version)

### Get the source code


$ git clone https://github.com/firebase/emulators-codelab.git
Then move into the codelab directory, where you will work for the remainder of this codelab:


$ cd emulators-codelab/codelab-initial-state
Now, install the dependencies so you can run the code. If you're on a slower internet connection this may take a minute or two:


# Move into the functions directory
$ cd functions

# Install dependencies
$ npm install

# Move back into the previous directory
$ cd ../

### Get the Firebase CLI
The Emulator Suite is part of the Firebase CLI (command-line interface) which can be installed on your machine with the following command:

```
  npm install -g firebase-tools@9.6.0
```
Next, confirm that you have the latest version of the CLI. This codelab should work with version 9.0.0 or higher but later versions include more bug fixes.

```
  $ firebase --version
  9.6.0
```
Connect to your Firebase project
If you don't have a Firebase project, in the Firebase console, create a new Firebase project. Make a note of the Project ID you choose, you will need it later.

Now we need to connect this code to your Firebase project. First run the following command to log in to the Firebase CLI:

```
  firebase login
```
Next run the following command to create a project alias. Replace $YOUR_PROJECT_ID with the ID of your Firebase project.

```
 firebase use $YOUR_PROJECT_ID
```
