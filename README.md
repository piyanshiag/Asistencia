# Asistencia

Asistencia is an attendance system which uses facial recognition to mark the in-time, and out-time of employees. It covers areas such as facial detection, alignment, and recognition, along with the development of a web application to cater to various use cases of the system such as registration of new employees, addition of photos to the training dataset, viewing attendance reports, etc. Admin can view attendance reports by using filters based on employee name and date. User can also their attendance using filters.
There are various graphs indicating the attendance reports of employees.

### Refer to this for admin user id and password.

## Technologies:
1. Python
2. Django
3. HTML
4. CSS
5. Javascript

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
   ```
   pip install -r requirements.txt
   ```
5. Run the application 
   ```
   python manage.py runserver
   ```
