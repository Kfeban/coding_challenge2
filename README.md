# Coding_challenge2
# Deploying the solutions I came up with in coding challenge 1, on to my assigned AWS server.
## i-Introduction
This project aims to deploy code solutions as a web interface using AWS server and Apache web server software.
The objective of this project is to provide a user-friendly way for users to interact with code solutions without modifying the original code. The web interface allows users
to input parameters for the code and view the results through a web browser.


## ii.Table on content
- i. Introduction
- ii. Table of content
- iii. Approach
- iv. Features
- v. Preeiquisities
- vi. setup
- vii. Usage
- viii. Results/output
- ix. Conclusion
    -  Comparisom of Implemented Solution with the Initial Plan
    -  challenges, or unexpected outcomes in the documentation
    -   analysis of the variations between the plan and the actual results
       
## iii-Approach methodolgy
To archieve our task ,we cam use the following approaches;

- [x] ***3.1 Server side scripting***(Approach we will be using for this sudies)
      
Utilize a server-side scripting language like Python, PHP, or Node.js to receive input from the user, execute the code on the server, and display the results.
This approach involves creating a web form that sends the user's input to the server, where the server-side script processes it and runs the code using the provided parameters.
The results are then returned to the user.
RESTful API:
- [x] ***RESTful API***
      
Develop a RESTful API that allows clients to send requests with the necessary parameters and receive the results.

<p>Representational State Transfer (REST) is a software architecture that imposes conditions on how an API should work.
  REST was initially created as a guideline to manage communication on a complex network like the internet. You can use REST-based architecture to support high-performing and reliable communication at scale. You can easily implement and modify it,
  bringing visibility and cross-platform portability to any API system.</p>

 ***How do RESTful APIs work?*** <P>
The basic function of a RESTful API is the same as browsing the internet. The client contacts the server by using the API when it requires a resource. API developers explain how the client should use the REST API in the server application API documentation. These are the general steps for any REST API call:

1. The client sends a request to the server. The client follows the API documentation to format the request in a way that the server understands.
2. The server authenticates the client and confirms that the client has the right to make that request.
3. The server receives the request and processes it internally.
4. The server returns a response to the client. The response contains information that tells the client whether the request was successful. The response also includes any information that the client requested.

This approach involves creating API endpoints that handle incoming requests, execute the code with the provided parameters, and respond with the results.
Clients can interact with the API using HTTP methods like POST or GET.

## iv-Features

- Web interface for deploying code solutions.
- Input form for users to provide parameters.
- Server-side script to execute the code with the provided parameters.
- Display of code results in the web browser.

  
## v-Prerequisites

To run this project, I'll need the following prerequisites:

- An AWS server with Ubuntu .
- Apache web server installed and configured on the AWS server.
- Basic knowledge of HTML, scripting language (e.g., Python, PHP, Node.js), and Apache configuration.

  ## vi-Setup

1. Set up AWS Server:
   - Sign in to the AWS Management Console.
   - Create a new EC2 instance with Ubuntu 20.04 LTS.
   - Assign a security group allowing inbound traffic on ports 22 (SSH) and 80 (HTTP).
   - Note down the public IP address of the server for future reference.
     ****estimated time 1hour****
     
2. Connect to the Server:
   - Open a terminal or command prompt on your local machine.
   - Use SSH to connect to the AWS server using the public IP address and the key pair associated with the instance.
     ****estimated time 3hour****
3. Install and Configure Apache:
   - Update the package lists on the server by running: `sudo apt update`.
   - Install Apache web server by running: `sudo apt install apache2`.
   - Start the Apache service by running: `sudo systemctl start apache2`.
   - Enable Apache to start on boot by running: `sudo systemctl enable apache2`.
     ****estimated time based on update speed 5hours****

4. Prepare Website Files:
   - Create a directory to store the website files, e.g., `/var/www/html`.
   - Transfer the original code files to the server using SCP or another file transfer method.
   - Place the code files in the appropriate directory on the server.
     ****estimated time 6hour****
     
5. Create a Simple Web Interface:
   - In the `/var/www/html` directory, create an HTML file, e.g., `index.html`.
   - Edit `index.html` using a text editor and add a web form for user input.
   - Add a submit button to send the form data to a server-side script.
   - Create a server-side script (e.g., using Python, PHP, Node.js) to process the form data, execute the code, and return the results.
      ****estimated time 6hours****
     
6. Configure Apache to Serve the Website:
   - Open the Apache configuration file for editing: `sudo nano /etc/apache2/sites-available/000-default.conf`.
   - Modify the document root to point to the directory with the website files, e.g., `DocumentRoot /var/www/html`.
   - Save the file and exit the text editor.
   - Restart Apache for the changes to take effect: `sudo systemctl restart apache2`.
     ****estimated time 3hours****

## vii-Usage

1. Open a web browser and enter the public IP address of the AWS server.
2. The web interface should be displayed with the input form.
3. Fill in the necessary parameters in the form.
4. Submit the form to execute the code with the provided parameters.
5. The results should be displayed in the web browser.

## viii-Results/Output

## ix-Conclusion


****READme file Updating****


****Comparisom of Implemented Solution with the Initial Plan****


Reflection on the proposed plan and compare it with the actual implementation.


****challenges, or unexpected outcomes in the documentation****


****analysis of the variations between the plan and the actual results****



