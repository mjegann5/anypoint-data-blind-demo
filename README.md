# anypoint-data-blind-demo

## How to usee this demo app

1. Clone the repo to your desktop

2. Import the project into Anypoint Studio

3. Get the temporary datablind.repo.authtoken from Kavi Software

5. Run the following command at the project root: 

    mvn -s settings.xml -Ddatablind.repo.authtoken=*********************** install

    This will install the required reepositories

6. Run the Mule Application in Anypoint studio

7. Use the postman collection to send a request to Demo App

    Compare the request and response JSON messages. The response JSON will show the encrypted fields. 
