**1- The two microservices are running and registered (two terminals, logs screenshots)**

    Account Service running
   ![Registration Service](images/AccountServiceTerminal.JPG)
   ![Registration Service](images/AccountServerInterfaz.JPG)
    
    Web Service running
   ![Registration Service](images/WebServiceTerminal.JPG)
   ![Registration Service](images/WebServiceInterfaz.JPG)
       
    
**2- The service registration service has the two microservices registered** 
    ![Registration Service](images/TwoMicroservicesEurekaInterfaz.JPG)
    ![Registration Service](images/TwoMicroservicesEurekaTerminal.JPG)
    
**3- A second account microservice is running in the port 4444 and it is registered**
    Account Service 2 running
   ![Registration Service](images/AccountService2Terminal.JPG)
   ![Registration Service](images/AccountServer2Interfaz.JPG)
    
    Account Service 2 registered
   ![Registration Service](images/TwoMicroservicesEureka2.JPG)
    
**4- A brief report describing what happens when you kill the microservice with port 2222. Can the web service provide information about the accounts? Why?**   
    Return an error message of connection refused, when the Web Server in port 333 connects to the microservice
    in port 2222.So when you try to connect again, when it tries to connect again it 
    asks to the Eureka Registration Server for the Account Service's address and  it 
    gets the right port 4444.