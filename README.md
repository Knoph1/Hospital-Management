# Hospital Management
![developer](https://img.shields.io/badge/Developed%20By%20%3A-Knoph%20A.-red)
[developer](https://github.com/Knoph1)
---
## screenshots
### Homepage
![homepage snap](https://github.com/sumitkumar1503/hospitalmanagement/blob/master/static/screenshots/homepage.png?raw=true)
### Admin Dashboard
![dashboard snap](https://github.com/sumitkumar1503/hospitalmanagement/blob/master/static/screenshots/admin_dashboard.png?raw=true)
### Invoice
![invoice snap](https://github.com/sumitkumar1503/hospitalmanagement/blob/master/static/screenshots/invoice.png?raw=true)
### Doctor list
![doctor snap](https://github.com/sumitkumar1503/hospitalmanagement/blob/master/static/screenshots/admin_doctor.png?raw=true)
---
## Functions
### Admin
- Sign up their account, Log in (no approval required).
- Can register/view/approve/reject/delete doctor (approve those doctor who applied for job in their hospital).
- Can admit/view/approve/reject/discharge patient (discharge patient when treatment is done).
- Can generate/download invoice pdf (generate Invoice according to medicine cost, room charge, doctor charge and other charge).
- Can view/book/approve appointment (approve those appointments which is requested by patient).

### Doctor
- Apply for job in hospital, Log in (approval required by hospital admin, then only doctor can login).
- Can only view their patient details (symptoms, name, mobile ) assigned to that doctor by admin.
- Can view their discharged (by admin) patient list.
- Can view their appointments, booked by admin.
- Can delete their appointment, when doctor attended their appointment.

### Patient
- Create account for admit in hospital, Log in (approval required by hospital admin, then only patient can login).
- Can view assigned doctor's details like (specialization, mobile, address).
- Can view their booked appointment status (pending/confirmed by admin).
- Can book appointments (approval required by admin).
- Can view/download invoice pdf (only when that patient is discharged by admin).

---

## HOW TO RUN THIS PROJECT
- Install Python(3.7.6) (dont forget to Tick Add to Path while installing Python)
- Open Terminal and execute the following Commands :
```
pip install django==3.0.5
pip install django-widget-tweaks
pip install xhtml2pdf
```
- Download this Project zip folder and extract it
- Move to project folder in Terminal, then run following Commands:
```
py manage.py makemigrations
py manage.py migrate
py manage.py runserver
```
- Now enter following URL in your browser installed on your PC
```
http://127.0.0.1:8000/
```

## CHANGES REQUIRED FOR CONTACT US PAGE
- In settins.py file, you have to give your email and password
```
EMAIL_HOST_USER = 'youremail@gmail.com'
EMAIL_HOST_PASSWORD = 'your email password'
EMAIL_RECEIVING_USER = 'youremail@gmail.com'
```
- Login to gmail through host email id in your browser and open following link and turn it ON
```
https://mail.google.com/mail/u/0/?tab=rm&ogbl#inbox
```
## Drawbacks/LoopHoles
- Any one can be Admin. There is no approval required for Admin account. So you can disable admin signup process and use any logic like creating Super_User.
- There should be at least one doctor in hospital before admitting patient. So first add doctor.
- On update page of doctor/patient you must have to update password.

## Disclaimer
This project is developed for demo purpose and it's not supposed to be used in real application.

## Feedback
Any suggestion and feedback is welcome. You can message me on facebook
- [Contact on Instargram](https://www.instagram.com/knoph_ol_a)
- [Contact on LinkedIn](https://www.linkedin.com/in/knoph-ayieko-83464918a)

## Work in progress, for a final release
