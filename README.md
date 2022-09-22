# anypoint-data-blind-demo

## Steps to use this demo app

1. Clone the repo to your desktop

2. Import the project into Anypoint Studio

3. Get a trial token from Kavi Software. This will be the value for datablind.repo.authtoken in the mvn command.

5. Run the following command at the project root: 

    mvn -s settings.xml -Ddatablind.repo.authtoken=*********************** install

    This will install the required repositories

6. In Anypoint Studio, Run the Demo as a Mule Application

7. Use the postman collection to send a request to Demo App

    Compare the request and response JSON messages. The response JSON will show the encrypted fields. 
