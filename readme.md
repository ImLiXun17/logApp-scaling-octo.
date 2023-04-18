# **LOG-APP**

## **Description** 

A log app is a software application that provides a centralized platform for collecting, storing, analyzing, and managing log data. Logs are records of events, messages, and actions that occur within an IT infrastructure, including servers, networks, applications, and security devices.

The purpose of a log app is to make it easier for IT administrators to monitor and troubleshoot their systems by providing a consolidated view of log data. The app collects logs from multiple sources and stores them in a searchable and filterable database. This allows administrators to quickly find specific log entries and identify patterns or trends in system behavior.

## **Visuals** 
![This is the visual of logApp](https://i.pinimg.com/564x/61/93/8e/61938ec7fa9121ba2730d91180136303.jpg)

## **Installation** 

### Download Xampp to set your server and database.
[Xampp Link Download](https://www.apachefriends.org/download.html)
![Image](https://1.bp.blogspot.com/-LRsqmuaX9Q0/XhhZfDGmkYI/AAAAAAAAAeo/Yhg_wi79pE03FituFE0Y0gKJ7FBKV_ihQCLcBGAsYHQ/s1600/xampp-virtual-host.png)


### Create a new database for your application.
![Image](https://installatron.com/images/remote/ss2_phpmyadmin.png)

### Set-up Your Database:
```
<?php
	define('ROOT_URL', 'http://localhost/logApp-scaling-octo/index.php');
	define('DB_HOST', 'localhost');
	define('DB_USER', 'root');
	define('DB_PASS', '');
	define('DB_NAME', 'logapp_usersdb');
	?>
```
### Establish Connection:
```
<?php
	// Create Connection
	$conn = mysqli_connect(DB_HOST, DB_USER, DB_PASS, DB_NAME);

	// Check Connection
	if(mysqli_connect_errno()){
		// Connection Failed
		echo 'Failed to connect to MySQL '. mysqli_connect_errno();
	}
	?>
```
### Use require method to Insert connection:
```
require('config/config.php');
require('config/db.php');
```
### Start application:
```
Start with your html and css with the following step above
```
## **Authors** 

+ [Maurene LLado-Github Account](https://github.com/ImLiXun17)
![image](https://scontent.fmnl3-1.fna.fbcdn.net/v/t39.30808-6/340488007_578911070873425_6032737004131118278_n.jpg?stp=dst-jpg_p526x296&_nc_cat=110&ccb=1-7&_nc_sid=730e14&_nc_eui2=AeFpc6lScjE3fqhMXpHsTljHoiWhKjMVwmyiJaEqMxXCbAY0QW0woMzw4FlYVm2blBzcXGeA2J0bCeoVZVJcg1w-&_nc_ohc=5l1hiJEigYkAX_SHAMJ&_nc_ht=scontent.fmnl3-1.fna&oh=00_AfB9KWTcyEHxCfQjlSeIM8DvQmvALF3vC-iPcOmkPjANIw&oe=6441D719) 

+ [Sean Harvey Orga-Github Account](https://github.com/SeanHarvy)
![image](https://avatars.githubusercontent.com/u/123426050?v=4)





