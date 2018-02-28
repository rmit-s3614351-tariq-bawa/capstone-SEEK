# capstone-SEEK

As the application sends search requests to the SEEK API hosted elsewhere, the modern browsers need authorization from the server to prevent Cross Origin Request Forgery. Therefore, they prevent it from accessing the SEEK API unless the following headers are included in the response from the API.

**Access-Control-Allow-Origin: {app_origin}**

As the SEEK API is merely an elasticsearch instance, this could be achieved using a proxy server such as nginx that intercepts the response to add the relevant headers to the response from Elasticsearch. For security reasons, it is recommended that the API does not allow any origin to send cross origin requests to it, as it can result in attacks against the elasticsearch index.

**Getting Started**

The following instructions mentioned in this user manual will get you a copy of the project up and running on your local machine for development and testing purposes.

**Prerequisites**
1.	System requirements:
A Windows/ Linux/ Mac computer with an internet connection¬

2.	Web Browser:
Preferably a modern web browser i.e. Google Chrome, Safari, Mozilla Firefox

3.	XAMPP
- Visit the following link https://www.apachefriends.org/download.html
- Download XAMPP version (v3.2.2)
- Open the downloaded file
- Follow the step by step installation wizard to successfully install XAMPP to your system

**Installing**
1.	Visit the following link: https://raw.githubusercontent.com/rmit-s3614351-tariq-bawa/SEEK/master/SEEK%20updated.zip
2.	The workspace (zip) file will begin to download automatically
3.	Locate the htdocs folder in the XAMPP application folder installed in your system. The common default path is as follows:
Windows: C:\xampp\htdocs
Linux: /opt/lampp/htdocs
Mac: /Applications/XAMPP/xamppfiles/htdocs

4.	Extract the cloud 9 workspace (which was downloaded in step 2) in to the htdocs folder
5.	Open the XAMPP application and click on the start button for Apache
6.	Open the config.json file with a text editor and make necessary changes by adding appropriate values to suit your environment e.g. server name, port
7.	Open the internet browser in your system and type “localhost” to run it on your local machine

**Running the tests**
•	Tests can be performed by changing the values in the config.json file to ensure the code is functional after the relevant changes
•	The job ID is implemented to be visible in both, search results and individual job description to ensure the linking between both json files are working as desired
•	Selenium automated browser tests

**Built With**
•	HTML
•	CSS
•	JavaScript
•	JSON
•	jQuery 3.3.1

**Authors**
•	Tariq M Bawa – Initial work – SEEK Search Engine

**Contributors:**
•	Leo Fitzgerald
•	Jason Yousif
•	Kaan Beyazbayram
