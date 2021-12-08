# /status

## Scenario 1 Validate GET status endpoint Total Requests
"GIVEN when the application is launched
WHEN port is set
WHEN  Enter the endpopint with password in the Terminal "/hash"
WHEN wait for 5 seconds
WHEN computes and returns Encripted Password
WHEN Enter GET status end point "/stats"
THEN Verify System return Total Requests user ran.
THEN Verify system returns the average time of a hash request in milliseconds since the server started."

## Defect TotalRequest is wrong 

## Scenario 2 Validate GET status endpoint average time using online tools
"GIVEN when the application is launched
WHEN port is set
WHEN  Enter the endpopint with password in the Terminal "/hash"
WHEN wait for 5 seconds
WHEN computes and returns Encripted Password
WHEN Enter GET status end point "/stats"
THEN System return Total Requests user ran.
THEN Verify system returns the average time of a hash request in milliseconds since the server started."

## Defect TotalRequest is wrong and AverageTime is wrong when converted

## Scenario 3 Validate Get the status end point when wrong port given in the end point
"GIVEN when the application is launched
WHEN port is set wrong
WHEN  Enter the endpopint with password in the Terminal "/hash"
WHEN wait for 5 seconds
WHEN computes and returns Encripted Password
WHEN Enter GET status end point "/stats"
THEN System return Total Requests user ran.
THEN system returns the average time of a hash request in milliseconds since the server started."

## Defect Connection refused

## Shutdown

## Scenario 1 Validate "Shutdown" endpoint 
"GIVEN when the application is launched 
WHEN port is set 
WHEN user enter POST endpoint shutdown /hash
THEN" Verify client and server got disconnected and when user tried running another endpoint

## Scenario 2 Validate Running Multiple Shutdown endpoint at the same time using &&
"GIVEN when the application is launched 
WHEN port is set 
WHEN user enter POST endpoint shutdown /hash && /hash
THEN" Connection refused when user tried running another endpoint

## Scenario 3  Validate Get the status end point having wrong port
"GIVEN when the application is launched 
WHEN wrong port is set 
WHEN user enter POST endpoint shutdown /hash 
THEN Connection refused 
