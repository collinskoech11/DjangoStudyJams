# DjangoStudyJams
Getting started with django tutorial session
## Requirements
- [x] Python3 installed 
## Proposed Workflow
- [x] Python 3 Installation
- [x] installing virtualenv 
- [ ] setting up virtual environment
- [ ] installing Django 
## Setting up a basic project
- [ ] Set up django project 
- [ ] Create first Django application 
- [ ] Set up application in the main project(settings.py)
- [ ] set up template & static folders
## Getting started with specifics 
- [ ] set up header and footer design in index view 
- [ ] set up views & urls for proposed views 
## Database (DBsqlite3 -> django default database)
- [ ] set up models for the various tables (i.e including foreign keys)
- [ ] import models to admin view 
- [ ] set up django workflow with github actions 
    - [ ] automate database migrations 


    ### Proposed tables 
    #### Users(extension)
    | fieldname | datatype | 
    | :-- | :-- | 
    | **username** | FK=> Users(User)  | 
    | **role** | VarChar(UserGroup)  | 
    | **user_id** | IntegerField  | 
    
    
    #### Inventory(meds)
    | fieldname | datatype | 
    | :-- | :-- | 
    | **med_name** | CharField  | 
    | **med_id** | IntegerField(AutoIncrement)  | 
    | **manufacturer** | IntegerField(AutoIncrement)  | 
    | **medtype** | CharField  | 
    | **dosage** | CharField  | 
    
     #### Symptoms -> Medical service request (Patients)
    | fieldname | datatype | 
    | :-- | :-- | 
    | **patient_name** | CharField(FK Users(User)  | 
    | **patient_id** | IntegerField(FK Users(User_id))  | 
    | **patient_age** | INtegerField  | 
    | **symptom** | CharField | 
    | **Duration of symptoms ** | IntegerField  | 
    
    
    #### Payments (Patients)
    | fieldname | datatype | 
    | :-- | :-- | 
    | **patient_name** | CharField(FK Users(User)  | 
    | **patient_id** | IntegerField(FK Users(User_id))  | 
    | **amount** | IntegerField  | 
    | **payment_id** | IntegerField(AutoIncrement)  | 
    
    #### Prescriptions (Medical Staff)
    | fieldname | datatype | 
    | :-- | :-- | 
    | **patient_name** | CharField(FK Users(User)  | 
    | **patient_id** | IntegerField(FK Users(User_id))  | 
    | **staff_name** | CharField(FK Users(User)  | 
    | **staff_id** | IntegerField(FK Users(User_id))  | 
    | **amount** | IntegerField  | 
    | **payment_id** | IntegerField(AutoIncrement)  | 




## User authentication & user groups 
- [ ] set up name & password verification 
- [ ] set up the diferent user groups 

## Design Implementation Intention 
- [ ] Login/Register
- [ ] Dashboard(Patient, Medical Staff)
- [ ] Medical Service Request(Symptoms Form -> Patients)
- [ ] Make Payments( -> Patients) 
- [ ] Check Medical service Requests( -> Medical staff)
    - [ ] Make Prescription based on selected service request(-> Medical staff)
    ### Dashboard design 
    - [ ] Patient Dashboard 
        - [ ] display patient name 
        - [ ] display payment history
        - [ ] display Medical history 
        - [ ] View all prescription with my name (Order by date)
    - [ ] Medical staff Dashboard 
        - [ ] Display staff name 
        - [ ] display presccription history  
        - [ ] display unattended requests 



## Views 
### Patients 
- [ ] Request Medical attention 
- [ ] Make payment 
- [ ] Display Payment history 
- [ ] Display Medical History 
### Medical Staff 
- [ ] View Medical attention requests 
- [ ] Make prescription 
- [ ] Prescriptions history 
