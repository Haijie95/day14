# Workshop 14

## How to start redis?
1. Start a redis server
```
wsl             -> For windows to use linux simulation
redis-server    -> To Start Server (on 1st tab)
```
2. To connect to redis server
```
wsl         -> For windows to use linux simulation
redis-cli   -> connect to server (on new tab)
```
3. Can proceed as usual to use mavern to run app
```
mvn spring-boot:run
```

## How to submit!
* Start railway init and go to settings
```
-> railway init
-> Add redis database
-> Copy the variable name & value in the railway
-> Mainly the username, password, port, host(end URL)
-> Paste it in the application properties
```
## This is for REDISDOTCOM
```
-> Go to redis official website 
-> Login
-> Go and open up a db
-> Get the username, password and host(URL)
-> Add them to the railway variable
-> Replace them with dynamic variables in the application.properties
```
## This is for branching
1. To branch out (change branch)
```
git checkout -b haijie

Purpose is to work on a version while not touching the present version
So as not to touch the Main
```
2. To return to main
```
git checkout main
```
## How to add mvn dependency for redis
```
Google mvn repository and search for redis

<!-- https://mvnrepository.com/artifact/redis.clients/jedis -->
		<dependency>
			<groupId>redis.clients</groupId>
			<artifactId>jedis</artifactId>
			<version>3.9.0</version>
		</dependency>
```
## Basic redis demo
* Pinging to check connection
```
redis-cli -h localhost ping
->  will get pong

keys *
->  get key value

set email k@k.com
->  key: email value: k@k.com

set count 1
->  key: count value: 1

keys *
->  will return all keys
1. email
2. count

get email 
->  will get email

del email
->  delete email

exists email
->  OK
incr count / incrby ##
->  return the increased count by 1

decrby count 10 / decr
->  return count minus 10

lpush cart apple
-> add apple into cart from the left

lindex cart 0
->  get cart index 0 item
```
