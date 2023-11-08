# anypoint-data-blind-demo

In order to use this demo app, you should first publish the [Data Blind connector](https://github.com/mjegann5/anypoint-data-blind-connector) in your exchange. Please visit [Data Blind connector](https://github.com/mjegann5/anypoint-data-blind-connector) for instruction for publishing.

## Steps to use this demo app

1. Clone the repo to your desktop

2. Import the project into Anypoint Studio 
        Studio version : v7.12.1
        Maven: Embedded Maven v3.6.3
        Java: Embedded Java JDK 8

3. In pom.xml, modify the value for datablind.exchange.groupId

    <datablind.exchange.groupId> PUT YOUR ANYPOINT GROUP ID <datablind.exchange.groupId>

4. Get a trial token from Kavi Software. This will be the value for datablind.repo.authtoken in the mvn command.

5. Run the following command at the project root:
   
   (anypoint_username & anypoint_password is required for accessing the anypoint account where you have published the connector.)

    mvn -s settings.xml -Ddatablind.repo.authtoken=*********************** -Danypoint_username=************ -Danypoint_password=*********** install

    This will install the required repositories.

6. In Anypoint Studio, Run the Demo as a Mule Application

7. Use the postman collection to send a request to Demo App

    Compare the request and response JSON messages. The response JSON will show the encrypted fields. 
