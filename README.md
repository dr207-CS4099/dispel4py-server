### Server Installation and Execution
Open a new terminal with the new `Laminar` directory.
```
/data/Laminar> 
```
Clone the server application repository.
```
/data/Laminar> git clone https://github.com/dr207-CS4099/dispel4py-server.git
```
update dispel4py-server/src/main/resources/application.properties to point to the appropriate database
To create a new database on the cs host servers:
```
mysql -u <username>
CREATE DATABASE <username>_Laminar;
```
To retrieve database connection settings:
```
mysql-initial-settings
```

Enter the server directory.
```
/data/Laminar> cd dispel4py-server
```
To manage permission issues, run:
```
/data/Laminar/dispel4py-server> chmod +x gradlew
```
To run the server (Linux)
```
/data/Laminar/dispel4py-server> ./gradlew bootRun
```
To run the server (Windows)
```
/data/Laminar/dispel4py-server> gradlew bootRun

The server will now be running, and ready to receive requests. You should see this sample output
```
/data/Laminar/dispel4py-server>
...
com.dispel4py.rest.RestApplication: Started RestApplication in 66.905 seconds (JVM running for 69.911)
...
