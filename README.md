# Asistencia

Asistencia is an attendance system which uses facial recognition to mark the in-time, and out-time of employees. It covers areas such as facial detection, alignment, and recognition, along with the development of a web application to cater to various use cases of the system such as registration of new employees, addition of photos to the training dataset, viewing attendance reports, etc. Admin can view attendance reports by using filters based on employee name and date. User can also their attendance by date.
There are various graphs indicating the attendance reports of employees.

### Refer to [this] for admin user id and password. 
[this]: https://github.com/piyanshiag/Asistencia/blob/master/automatic_attendance/passwords.txt

### Tools and languages:
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white) ![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E) ![Django](https://img.shields.io/badge/django-%23092E20.svg?style=for-the-badge&logo=django&logoColor=white) ![OpenCV](https://img.shields.io/badge/opencv-%23white.svg?style=for-the-badge&logo=opencv&logoColor=white) ![Bootstrap](https://img.shields.io/badge/bootstrap-%23563D7C.svg?style=for-the-badge&logo=bootstrap&logoColor=white) ![SQLite](https://img.shields.io/badge/sqlite-%2307405e.svg?style=for-the-badge&logo=sqlite&logoColor=white) 


### We have 2 types of users of the system.
1. Employee
2. Admin

### Following functionalities can be performed by the admin: 
*  Login 
*  Register new employees to the system
*  Add employee photos to the training data set
*  Train the model
*  View attendance report of all employees. Attendance can be filtered by date or employee.

### Following functionalities can be performed by the employee: 
* Login
* Mark his/her time-in and time-out by scanning their face 
* View attendance report of self

## Face Detection
Dlib's HOG facial detector.

## Facial Landmark Detection
Dlib's 68 point shape predictor

## Extraction of Facial Embeddings
face_recognition by Adam Geitgey

## Classification of Unknown Embedding
using a Linear SVM (scikit-learn)

## Install and run the application 
1. Clone the repository 
2. Create an anaconda environment
   ```
   conda create -n myenv python=3.7 
   ```
3. Activate the environment and get inside folder automatic_attendance
4. Install the requirements
   For DLIB to work, install [visual studio] and then install **Desktop development with C++** while setting up Visual Studio
   
   [visual studio]: https://visualstudio.microsoft.com/
   
   Follow this [article] to install CMake and DLIB
   
   [article]: https://medium.com/analytics-vidhya/how-to-install-dlib-library-for-python-in-windows-10-57348ba1117f
   
   Next:
   ```
   pip install -r requirements.txt
   ```
5. Run the application 
   ```
   python manage.py runserver
   ```
