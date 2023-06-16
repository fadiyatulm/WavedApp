## Cloud Infrastructure
![CloudInfrastructure](https://github.com/fadiyatulm/WavedApp/blob/main/pic/infrastructure.png)

## Steps to Deploy in Google Cloud
1. Create Cloud Storage Bucket, make sure that you name it uniquely and the object can be viewed publicly.
2. Create Cloud SQL instance and choose MySQL 8.0 as a Database Engine. Then import waved.sql into it.
3. Open Navigation menu and choose App Engine.
4. Create Application and then choose region and also service account that will be used by App Engine.
5. Clone this repository
```
git clone https://github.com/fadiyatulm/WavedApp.git
```
6. Make sure you are on the CC directory.
7. Create .env file and insert the configuration below:
```
PORT= your port
ACCESS_TOKEN = your access token
DB_HOST = "your database host"
DB_USER = "your database user"
DB_PASSWORD = "your database password"
DB_NAME = "your database name"
```
8. Install dependencies such as express, bcrypt, mysql, cors, body-parser, dotenv, and jsonwebtoken.
9. Make an ```app.yaml``` file and enter ```nodejs16``` as a runtime.
10. Then deploy it by entering commands ```gcloud app deploy``` in terminal.

## Test the Endpoint in Postman
1. Enter the URL with ```https://waved-app.et.r.appspot.com/dictionary``` and select ```GET``` as a method.
2. You will get this as a result.
![Result](https://github.com/fadiyatulm/WavedApp/blob/main/pic/Screenshot%202023-06-15%20151818.png)



