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
### Feature
1. **Splash Screen.** There is logo screen before into the login page.
2. **Login.** Allows user to gain access to an application by entering their username and password.
3. **Register.** Enables user to independently register and gain access to the system.
4. **Home.** The start page that is displayed when you have logged in on your device.
5. **Take Image From Camera.** You can take image from camera in preparation for uploading an image to detect the means of the handsign.
6. **Article About Handsign.** In this application you can read informatin about handsign

### Dependencies
* Jetpack Compose
* Lifecycle & Livedata6
* kotlinx-coroutines
* Real-time
* Firebase

### Getting Started Application
- Prerequisites
  - Tools Software <br>
    a. Android Studio <br>
    b. JRE (Java Runtime Environment) or JDK (Java  Development Kit)

### Acknowledgements
* [Clean Architecture Guide](https://developer.android.com/jetpack/guide)
* [Android Application Fundamental](https://developer.android.com/guide/components/fundamentals)
* [Android Jetpack Pro](https://developer.android.com/jetpack)
* [Dependency injection](https://developer.android.com/training/dependency-injection)

## Machine Learning
### Dataset
We are using Bahasa Isyarat Indonesia (BISINDO)<br>
* [Alphabets](https://www.kaggle.com/datasets/achmadnoer/alfabet-bisindo)<br>
* [ISLBISINDO1](https://www.kaggle.com/datasets/idhamozi/indonesian-sign-language-bisindo)<br>
* [Bisindo Dataset](https://www.kaggle.com/datasets/yunitayupratiwi/bisindo-dataset)<br>
* And our self-made dataset.

### Method
Pre-trained InceptionV3

### Tools
* Tensorflow
* Numpy
* Pandas
* Matplotlib
* Pathlib
* Os
* Google Collab
* Visual Studio Code

### Predict
In this project we made our own dataset and combined in our local, the dataset
contains a 26 classes there are A, B, C, D, E, F, G, H, I, J, K, L, M, N, O, P,
Q, R, S, T, U, V, W, X, Y and Z. There are two directory dataset and datatrain.

### Deployment
We are using Tensorflow Lite to deploy the model on Android

### References
Load and processing data: https://www.kaggle.com/code/databeru/fruit-and-vegetable-classification

## Cloud Computing
### Cloud Infrastructure
![CloudInfrastructure](https://github.com/fadiyatulm/WavedApp/blob/main/pic/infrastructure.png)

### Steps to Deploy in Google Cloud
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

### Test the Endpoint in Postman
1. Enter the URL with ```https://waved-app.et.r.appspot.com/dictionary``` and select ```GET``` as a method.
2. You will get this as a result.
![Result](https://github.com/fadiyatulm/WavedApp/blob/main/pic/Screenshot%202023-06-15%20151818.png)



