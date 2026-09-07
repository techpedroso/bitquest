# BitQuest (formerly also known as QuestBit)

Reading the Application Source Code
To read and analyze the application's source code, any integrated development environment (IDE) compatible with the project's files may be used. However, the use of Visual Studio Code is recommended, as it provides features that facilitate the configuration and execution of the application.

Requirements for Running the Application
Before running the application, some tools must be installed and properly configured on the machine:

Visual Studio Code: the development environment used to edit and run the project. The Windows installer is available in the official documentation: https://code.visualstudio.com/docs/setup/windows

Node.js: the runtime environment required to execute the application's backend.

Node Package Manager (npm): the package manager used to install the project's dependencies. npm is installed together with Node.js. The Windows installer is available at: https://nodejs.org/pt/download/prebuilt-installer

The installation of Node.js and npm can be verified through the Command Prompt (CMD) by using the following commands:

node -v

The command above displays the installed version of Node.js.

npm -v

The second command displays the installed version of npm.

Obtaining the Source Code
After configuring the development environment, the source code can be obtained using the git clone command, which clones the repository to the local machine:

git clone https://github.com/devmpedroso/questbit.git

If Git is not installed on the machine, the project can also be obtained as a .zip file. To do so, access the project's repository on GitHub, select the Code option, and then choose the option to download the project as a ZIP file.

Directory Structure
It is important to preserve the application's directory structure after obtaining the project. The BACKEND and FRONTEND directories must remain at the root of the project, according to the structure originally defined for the application.

For example, if a folder is created on the desktop to store the project, the resulting structure should be similar to the following:

questbit/
├── BACKEND/
└── FRONTEND/

Therefore, additional directory levels that could alter the expected project structure should be avoided.

Installing the Dependencies
After obtaining the repository and verifying that the BACKEND and FRONTEND directories are correctly positioned at the project root, the dependencies required to run the application must be installed.

In Visual Studio Code, access the extensions panel by selecting the icon represented by four squares. In the search bar, search for the Live Server extension and install it.

The Live Server extension is used to make the frontend pages available locally.

Next, open the integrated terminal in Visual Studio Code. This can be done using the Ctrl + Shift + ' keyboard shortcut. Alternatively, the terminal can be accessed through the View > Terminal menu.

With the terminal open, navigate to the backend directory using the following command:

cd backend

After accessing the directory, run the following command to install the project's dependencies:

npm i

Once the installation is complete, the required dependencies will be available and the environment will be ready to run the application.

Running the Application
To start the application, open the integrated terminal in Visual Studio Code and verify that the current directory is the backend folder.

Then, execute the following command:

npm run dev

This command starts the server responsible for the application's backend. If the initialization is successful, the terminal will display information regarding the server's operation and the connection to the cloud-hosted database.

After starting the backend, the frontend must be started using the previously installed Live Server extension.

To do so, click the Go Live option located in the lower-right corner of the Visual Studio Code interface. This action starts a local server that makes the frontend pages available through a web browser.

Accessing the Registration Page
After starting the frontend, the browser may initially display a page containing the project's directories. In this case, navigate through the following structure:

frontend > pages > signup.html

The signup.html file corresponds to the application's registration page and can be used as the starting point for analyzing its features and navigation flow.

Unimplemented Features
During the analysis of the application, some features were identified as either not implemented or not intended to be accessed in the version provided for evaluation.

Date Page
The page related to the date functionality, identified by an arrow icon, should not be accessed, as this feature was not implemented in the current version of the application.

If the page is accessed accidentally, the user should return to the previous page.

Completed Tasks Chart
The chart responsible for displaying the number of completed tasks is also not implemented in the current version of the application.
