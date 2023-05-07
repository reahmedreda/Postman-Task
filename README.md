# Postman-Task


* The task is a basic api testing using postman. 
* The url : https://postman-echo.com

-------------------------------------------
## Basic Requirements : 
- Create a postman collection that contains automated tests for 2 end points  :
	1- GET https://postman-echo.com/basic-auth 
		This end point validates that the credentials were entered are correct . In order to call this end point you need to set the authentication
     to basic Auth 

		- valid credentials :
				username = postman
				password = password
			expected response : 
				{
			    	"authenticated": true
				}

		- Invalid credentials will fire a status code 401 Unauthorised 



	2- GET https://postman-echo.com/get
		This end point works as an echo , if you send it a query paramter it will show it in the response as an argument [ key and value ]

		ex : when calling 
		https://postman-echo.com/get?foo1=bar1&foo2=bar2

		the response will contain :
		 "args": {
		        "foo1": "bar1",
		        "foo2": "bar2"
		    },

- Write automated testcases for each endpoint to check the status codes and functionality , create as many test cases as you think is enough but don't over engineer 
- Create a shell script to Run the collection from command line , name it "testScript"

------------------------------------------

## Bonus Requirements : 
- [ 10 Points] Extract the base url, username and password to external file and pass it in the command line 

- [ 10 points ] Send the username and credentials directly from the command line directly as command arguments 

- [ 20 point ] Add the credentials to system enviroment variables and pass it to the command 

- [ 20 points] Generate junit xml report through the script command 


-----------------------------------------
## Delivering the task :

- Add all files in .zip and make sure to attach the shell script file . Note that the task will be ran through this shell script otherwise the task is invalid 
- send the zip file to email : ahmed.reda@pixelogicmedia.com
- The title of the email should be : "ITI_Internship_Task"
- attach your cv in the email 
- Deadline is on Monday 8th of May at 11:59 PM 
