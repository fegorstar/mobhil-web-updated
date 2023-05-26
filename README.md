
# About The Project
This is an used Car Selling Business Website for Mobhil cars company, where users can search and view details of car as well as make inquiry for the car they like. It is built with Python (django), HTML5, CSS3, JavaScript and Bootstrap.

<img src="https://github.com/fegorstar/mobhil-web/blob/master/mobhil/static/img/homepage.PNG">


## App Features
- Pages: which contains the homepage, about page and every other static pages.
- Cars: Which contains the cars listings and listing.
- Accounts: Which allows the users to register and login.
- Search functionality
- Contacts: which allows the user to fill a form to make inquiry about a car listing.


# Setup Instructions
1. Clone the repository `git clone https://github.com/fegorstar/mobhil-web-updated.git`
2. Navigrate to the working directory `cd mobhil-web-updated`
3. Open the project from the code editor `code .` or `atom .`
4. Create virtual environment `virtualenv venv`
5. Activate the virtual environment `source venv/Scripts/activate`
6. Install required packages to run the project `pip install -r requirements.txt`
7. Rename _.env-sample_ to _.env_
8. Fill up the environment variables:
    _Generate your own Secret key using this tool [https://djecrety.ir/](https://djecrety.ir/), copy and paste the secret key in the SECRET_KEY field._

    _Your configuration should look something like this:_
    ```sh
    SECRET_KEY=47d)n05#ei0rg4#)*@fuhc%$5+0n(t%jgxg$)!1pkegsi*l4c%
    DEBUG=True
    EMAIL_HOST=smtp.gmail.com
    EMAIL_PORT=587
    EMAIL_HOST_USER=youremailaddress@gmail.com
    EMAIL_HOST_PASSWORD=yourStrongPassword
    EMAIL_USE_TLS=True
    ```
    _Note: If you are using gmail account, make sure to [use app password](https://support.google.com/accounts/answer/185833)_
9. If you use pgAdmin4 GUI like me, you can open it and create a database. 
10. Then open your Settings.py file and the Database section, rename the database name to the one you just created.
11. To create your database tables, issue the commands below:
    ```sh
    python manage.py makemigrations
    ```

    ```sh
    python manage.py migrate
    ```
10. Create a super user
    ```sh
    python manage.py createsuperuser
    ```
    _GitBash users may have to run this to create a super user - `winpty python manage.py createsuperuser`_
11. Run server
    ```sh
    python manage.py runserver
    ```
12. Login to admin panel - (`http://127.0.0.1:8000/admin/`)
13. Add car listings, register user, login, and explore all the various features of the app.


## Support
💙 If you like this project, give it a ⭐ and share it with friends!

##
Made with ❤️ and Python
