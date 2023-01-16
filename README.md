* 1. Start a redis server
```
wsl             -> For windows to use linux simulation
redis-server    -> To Start Server (on 1st tab)
```
* 2. To connect to redis server
```
wsl         -> For windows to use linux simulation
redis-cli   -> connect to server (on new tab)
```
* 3. Can proceed as usual to use mavern to run app
```
mvn spring-boot:run
```

How to submit!
* 1. Start railway init and go to settings
```
-> railway init
-> Add redis database
-> Copy the variable name & value in the railway
-> Mainly the username, password, port, host(end URL)
-> Paste it in the application properties
```
* This is for REDISDOTCOM
```
-> Go to redis official website 
-> Login
-> Go and open up a db
-> Get the username, password and host(URL)
-> Add them to the railway variable
-> Replace them with dynamic variables in the application.properties
```
