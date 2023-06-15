# WavEd
<p align="center">
 <img src="https://github.com/fadiyatulm/WavedApp/blob/main/pic/logo.png" alt="Project logo"></a>
</p>
<p align="center">
C23-PS318’s Capstone repository
</p>

## Our Team Members
| Name                      | Bangkit ID  | Path                |
|  :--------------------:   |  :------:   | :------------:      |
| Hana Zhafirah             | M037DSY1275 | Machine Learning    |
| Raihan Mufadhdhol Jefri   | M037DSX1437 | Machine Learning    |
| Adam Haidar Dzaky Tanjung | A322DKX3864 | Mobile Development  |
| Andi Fadgham Izza Rizky   | A062DSX1720 | Mobile Development  |
| Widya Titah Pertiwi       | C287DKY3824 | Cloud Computing     |
| Fadiyatul Muqtashidah     | C287DKY3811 | Cloud Computing     |

## Our Project
WavEd is an application for learning Bahasa Isyarat Indonesia or BISINDO (Indonesian Sign Language). WavEd has a gamification feature. User will
demonstrate the BISINDO and then the application will predict whether their movement is correct or not. User can learn the BISINDO’s words through
the dictionary feature.

## Mobile Development

## Machine Learning

## Cloud Computing
### Cloud Infrastructure
![CloudInfrastructure](https://github.com/fadiyatulm/WavedApp/blob/main/pic/infrastructure.png)

### Steps to Deploy in Google Cloud
1. Create Cloud Storage Bucket, make sure that you name it uniquely and the object can be viewed publicly.
2. Create Cloud SQL instance and choose MySQL 8.0 as a Database Engine. Then import waved.sql into it.
3. Open Navigation menu and choose App Engine
4. Create Application and then choose region and also service account that will be used by App Engine
5. Clone this repository
```
git clone https://github.com/fadiyatulm/waved.git
```
6. Create .env file and insert the configuration below:
```
PORT= your port
ACCESS_TOKEN = your access token
DB_HOST = "your database host"
DB_USER = "your database user"
DB_PASSWORD = "your database password"
DB_NAME = "your database name"
```
7. Install dependencies such as express, bcrypt, mysql, cors, body-parser, dotenv, and jsonwebtoken.
8. Then deploy it by entering commands ```gcloud app deploy``` in terminal and make sure you are on the waved directory.

### Test the Endpoint in Postman
1. Enter the URL with ```https://waved-app.et.r.appspot.com/dictionary``` and select ```GET``` as a method.
2. 



