The two microservices are running and registered (two terminals, logs screenshots).

 -As seen on screenshots "accounts_1" and "web".
 
The service registration service has the two microservices registered (a third terminal, dashboard screenshots)

 -As seen on screenshot "dashboard".
 
A second account microservice is running in the port 4444 and it is registered (a fourth terminal, log screenshots).

 -As seen on screenshots "accounts_2" and "dashboard(2 accounts)".
 
A brief report describing what happens when you kill the microservice with port 2222. Can the web service provide information about the accounts? Why?
 
 -If we kill the account service microservice in port 2222 the web server will return a connection refused message when asked for an account immediately.
  We'll have to wait for the web server to connect again (in this case to account service in port 4444) in order to get an account.
