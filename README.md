<p align="center">

  <h3 align="center">Website for Lunchtime Yoga for Professionals</h3>

  <p align="center">
    A mobile responsive website to allow users/instructors to create, schedule, and signup for yoga classes in Boise, Idaho.
    <br />
    <a href="https://yoga-website.herokuapp.com/">View Heroku Demo</a>  <a href="https://github.com/Bolmstead/Yoga"><strong>Explore the docs »</strong><a>
  </p>
</p>

![Website_pic](static/images/website.png?raw=true "website")

<!-- ABOUT THE PROJECT -->
## About The Project

This project was created as the Capstone 1 project for the Springboard Software Engineering Course. It will hopefully be used  operate as a website for the Lunchtime Yoga for Business Professionals group in the near future. While on the website, a user is able to do the following:
* View information about the group including pricing, instructor bios, how to contact, and social media links.
* Create and log into an account with an encrypted password using bcrypt.
* Signup for available yoga classes using the website's javascript calendar.
* View enrolled yoga classes and cancel any class signup.
* Edit their account information.
* (soon) Receive automatic emails to confirm their yoga class signup, signup cancellation, or account creation.


Instructors are able to do all of the above while having the ability to:
* Create/delete yoga classes.
* View who has enrolled for each class.


## Built With

The coding languages, frameworks, source code, and API that I used to build this project:
* Python
* Javascript
* HTML
* CSS
* [Bootstrap](https://getbootstrap.com)
* [JQuery](https://jquery.com)
* [Axios](https://www.npmjs.com/package/axios)
* [Jinja](https://jinja.palletsprojects.com/en/2.11.x/)
* [Flask](https://flask.palletsprojects.com/en/1.1.x/)
* [Postgres](https://www.postgresql.org/)
* [SQL Alchemy](https://flask-sqlalchemy.palletsprojects.com/en/2.x/)
* [Flask-Bcrypt](https://flask-bcrypt.readthedocs.io/en/latest/)
* [WTForms](https://wtforms.readthedocs.io/en/2.3.x/)
* [Font Awesome](https://fontawesome.com/)
* [Simple Calendar](https://github.com/brospars/simple-calendar)
* [Send Grid Email API](https://sendgrid.com/docs/api-reference/)


<!-- GETTING STARTED -->
## How to Run the Project

To get a local copy up and running follow these steps:

### Clone Repo

1. Clone the repo by clicking on the green "Code" button at the top of the github repo page or by entering the following in your terminal:
   ```sh
   git clone https://github.com/Bolmstead/Yoga.git
   ```
2. (optional but recommended) Create a [virtual environment](https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/) in the same directory of the cloned, unzipped code.

### Library Installations

3. Use the package manager [pip](https://pip.pypa.io/en/stable/) to install the requirements.txt.

  ```sh
  pip install -r requirements.txt
  ```

### Postgres Installation

4. Install [Postgres](https://www.postgresql.org/).
5. Create a database named "yoga" in your terminal.
  ```sh
  createdb yoga
  ```
6. Start a server in your projects directory and you are done!

<!-- ROADMAP -->
## Roadmap

Possible features that I would like to integrate into the website are:
* As requested by an instructor, an instructor could add any user to a class.
* Payment system to allow a user to pay/prepay for classes on the website.
* User having a class credits column that would deplete after they attend a class and can be refilled by an instructor if receive prepayments.
* Google calendar API that would allow a user to save their class signup to their google calendar. Also could be used for instructors when they create a class.


## Bugs to be fixed

A few bugs are still in the code and I am working to debug them:
* SendGrid Email API function is not currently working. While the working code is included and commented out in the ```sh app. py``` file, my account needs approval before the automatic confirmation emails can be sent again. Once my account is approved, the code will be uncommented. 
* Calendar sometimes doesn't show the colored circle on date of class, however the classes are still populating to the calendar and show after the date is clicked.
* Timezones of the start and end times of the classes are saved to the database in the GMT timezone rather than MST. I have a Javascript workaround to show the correct times in the calendar, but currently working to debug this.
<!-- LICENSE -->
## Notes
For the sake of the capstone code review, any user can sign up to be an instructor on the website. This just allows anyone to view the instructor's functionality. If this website were to be implemented, instructors accounts would be created in a different way requiring approval.

The source code for the calendar used on the website was pulled and maniputlated from [Simple Calendar](https://github.com/brospars/simple-calendar). Author of the Simple Calendar grants permission to any person to use, copy, modify, or publish the code. All documents regarding the Simple Calendar code are located in /static/calendar.

## Contact
Enjoy!

<!-- CONTACT -->
## Contact

Berkley Olmstead - olms2074@gmail.com - [Linkedin](https://www.linkedin.com/in/berkleyolmstead/)

Project Link: [https://github.com/Bolmstead/Yoga](https://github.com/Bolmstead/Yoga)
