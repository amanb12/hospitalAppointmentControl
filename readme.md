[![Build Status](https://github.com/amanb12/hospitalAppointmentControl/actions/workflows/master_hospital-appointment-control-system.yml/badge.svg?branch=master)](https://github.com/amanb12/hospitalAppointmentControl/actions/workflows/master_hospital-appointment-control-system.yml)
<br />
<a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-purple.svg?labelColor=303030" /></a>
<a><img alt="GitHub Forks" src="https://img.shields.io/github/forks/sumitkumar1503/hospitalmanagement?color=orange" /><a>
<br />

## About The Project

<div>
  <p>
    This django temolate is created by
    <a href="https://github.com/sumitkumar1503/hospitalmanagement">sumitkumar1503/hospitalmanagement.</a>
  </p>
</div>

I used this project to demonstrate my Microsoft Azure skills during the
<a href="https://futurereadytalent.in/">Future Ready Talent Program</a>.
The djano app is deployed on **Azure App Service** and the database is configured with **Azure Database for PostgreSQL**.

The project is a simple doctor appointment management system and allows you to manage medical appointments of a single or group of doctors by a centralized administration.
A patient can book an appointment with a doctor at their convinience and if it gets approved by the admins, the doctor can view the list of appointments of their patients.
As a sample, this project is not intended for commercial deployment.

<br />

## Functions

### Admin

<div>
  <a href="https://raw.githubusercontent.com/amanb12/hospitalAppointmentControl/master/static/screenshots/admin_dashboard.png">
    <img align="right" width="240px"  src="https://raw.githubusercontent.com/amanb12/hospitalAppointmentControl/master/static/screenshots/admin_dashboard.png">
  </a>
</div>

- Signup their account. Then Login (No approval Required).
- Can register/view/approve/reject/delete doctor (approve those doctor who applied for job in their hospital).
- Can admit/view/approve/reject/discharge patient (discharge patient when treatment is done).
- Can Generate/Download Invoice pdf (Generate Invoice according to medicine cost, room charge, doctor charge and other charge).
- Can view/book/approve Appointment (approve those appointments which is requested by patient).

### Doctor

- Apply for job in hospital. Then Login (Approval required by hospital admin, Then only doctor can login).
- Can only view their patient details (symptoms, name, mobile ) assigned to that doctor by admin.
- Can view their discharged(by admin) patient list.
- Can view their Appointments, booked by admin.
- Can delete their Appointment, when doctor attended their appointment.

### Patient

- Create account for admit in hospital. Then Login (Approval required by hospital admin, Then only patient can login).
- Can view assigned doctor's details like ( specialization, mobile, address).
- Can view their booked appointment status (pending/confirmed by admin).
- Can book appointments.(approval required by admin)
- Can view/download Invoice pdf (Only when that patient is discharged by admin).

## Drawbacks/LoopHoles

- Any one can be Admin. There is no Approval required for admin account. So you can disable admin signup process and use any logic like creating superuser.
- There should be at least one doctor in hospital before admitting patient. So first add doctor.
- On update page of doctor/patient you must have to update password.
