
# TODO:
* get color from color picker and pass to canvas
* Check why canvas hand isn't exactly aligned with drawing
* Add More Routes to back-end
* Check if login page route now works



# Running the Application

After installing the pre-reqs and following the local setup instructions listed below: 

* Open a terminal and navigate to the *Frontend* directory then run:
```
npm install 
npm start
```

* Open another terminal and navigate to the *Backend* directory then run: 
```
npm install 
node index.js
```

## Local

## Pre-reqs
* Install Flyway for database migrations.
	* MACOS: `brew install flyway`
	* or: https://flywaydb.org/download/ 

* Install Docker to run postgres image

### Setup
Run the local docker environment by going to the project root directory and running:

```$ cd docker-envs/local && docker-compose up```

Run the database migration scripts by going to the project root directory and running:

```$ scripts/migrate_all_local.sh```

## Database Configurations


| Host  |  Port | Database  | Username  | Password  |
|---|---|---|---|---|
| localhost  | 5434  | pictochatdb  | me  | password  |


## pictochatdb schema

Accounts
----------
user_id (PK)
email
password


Messages
----------
MessageID (PK)  
SenderID (FK)  
RecipientsID (FK)  
Subject  
ImageData
DateSent  

