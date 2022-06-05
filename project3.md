## PROJECT 3: MERN STACK IMPLEMENTATION
### SIMPLE TO-DO APPLICATION ON MERN WEB STACK

### STEP 1 – BACKEND CONFIGURATION

#### I'm to Update ubuntu with the command below
`sudo apt update`

![Ubuntu Update](images/sudoupdate.png)

#### I'm to upgrade ubuntu server with the command below
`sudo apt upgrade`

![Ubuntu Upgrade](images/sudoupgrade.png)

#### Lets Install Node.js on the server
#### Install Node.js with the command below

`sudo apt-get install -y nodejs`

![Install Node](images/installnode.png)

#### The command above installs both nodejs and npm. NPM is a package manager for Node like apt for Ubuntu, it is used to install Node modules & packages and to manage dependency conflicts.Verify the node installation with the command below

`node -v `

![Install Node](images/node.png)

#### Verify the node installation with the command below

`npm -v `
![Install NPM](images/npm.png)

#### Create a new directory for your To-Do project:
`mkdir Todo`

![Make Directory](images/mkdirtodo.png)

#### Run the command below to verify that the Todo directory is created with ls command
`ls`

![List Directory](images/mkdirtodols.png)

#### Now lets change our current directory to the newly created one:

`cd Todo`

![cd Todo](images/cdtodo.png)

#### Next,  I you will use the command npm init to initialise my project, so that a new file named package.json will be created. This file will normally contain information about my application and the dependencies that it needs to run. I will follow the prompts after running the command. I will press Enter several times to accept default values, then accept to write out the package.json file by typing yes.

`npm init`
![Init](images/init.png)


#### I will run the command ls to confirm that I have package.json file created. Next, I will Install ExpressJs and create the Routes directory.

## INSTALL EXPRESSJS

#### To use express, I will install it using npm:

`npm install express`

![Install Express](images/installexpress.png)

#### Now create a file index.js with the command below

`touch index.js`
![Create Index.Js File](images/touchindexjs.png)


#### Install the dotenv module

`npm install dotenv`

![Install Dotenv](images/installdotenv.png)

#### Open the index.js file with the command below

`vim index.js`

![Open Index.js](images/vimandcatindexjs.png)


#### Notice that I have specified to use port 5000 in the code. This will be required later when I go on the browser.

#### Now it is time to start our server to see if it works. I Open my terminal in the same directory as my index.js file and type:

`node index.js`

#### Now I see my Server running on port 5000 in my terminal

![Node Running](images/nodeindexjs.png)

#### I have enable port 80 on my AWS security group in other to access my server on the web

#### I Open up my browser and try to access my server’s Public IP or Public DNS name followed by port 5000:

![Web Running](images/runningonweb.png)

#### Routes
#### There are three actions that our To-Do application needs to be able to do:

#### 1. Create a new task
#### 2. Display list of all tasks
#### 3. Delete a completed task
#### Each task will be associated with some particular endpoint and will use different standard HTTP request methods: POST, GET, DELETE.

#### For each task, we need to create routes that will define various endpoints that the To-do app will depend on. So let us create a folder routes

`mkdir routes`
![Make Routes](images/makeroute.png)

#### Change directory to routes folder.
`cd routes`

![Make Routes](images/makeroute.png)

#### Now, create a file api.js with the command below
`touch api.js`
![Make Routes](images/makeroute.png)
#### Open the file with the command below

`vim api.js`

![VIM Route](images/vimandcatroute.png)
















