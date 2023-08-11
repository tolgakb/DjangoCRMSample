# DjangoCRMSample

In this project, CRUD operations in django is implemented. 

Registration, login and logout processes, which are the authentication processes, are performed.

In response to the user, for example, when they perform authentication operations or CRUD operations, information is given with django messages.

The attribute information of the records to be added is determined with the help of the Django model.


In the navbar, if the user is logged in, there are options to add record and logout, and if the user is not logged in, there are options to login and register.

If the user is not logged in on the main page, he completes the login process by filling out the username and password information with a form. 

![Screenshot_1](https://github.com/tolgakb/DjangoCRMSample/assets/101968167/d3689427-c298-405e-9ab8-49b49104d4b2)


If the user is logged in, the detailed information of the previously added records are listed with the help of the table.

![Screenshot_2](https://github.com/tolgakb/DjangoCRMSample/assets/101968167/225134b0-9d4b-4c0e-af4e-0733b75011b5)

We can access each of the records listed on the homepage separately with a link and direct them to the detail page. On the detail page, we list the recorded information and the user has the options to delete the record and update the record if they wish.
The user can delete the record by clicking the delete button on the detail page and a message that the record has been deleted is displayed on the homepage.

![Screenshot_3](https://github.com/tolgakb/DjangoCRMSample/assets/101968167/33636383-ec26-4b91-8f29-7ecf9d3c99fe)

On the Register page, a form with username, firstname, lastname, email address, password and password conformation fields are presented to the user to enter their information. This form is made by importing UserCreationForm from Django authentication forms. In the form, we add the fields we want to be in addition to the username, password1 and password2 in the User model. When the user submits the form, we check the form and if the form is valid, we save the form and after creating the new user, we complete the login process and redirect it to the home page.

![Screenshot_6](https://github.com/tolgakb/DjangoCRMSample/assets/101968167/c3b52696-ccd5-4e2a-8512-394403d8288a)

When the user wants to add a new record, we specify the fields we want to be in the form and present these fields to the user. When the user fills out the form and clicks the add new record button, we check the form, if the form is valid, we save the form and redirecting the user to the homepage, we inform the user that a new record has been added.

![Screenshot_5](https://github.com/tolgakb/DjangoCRMSample/assets/101968167/b07abc9c-ca2e-4ff9-ad07-6863275fa1a3)

When the update record button on the user detail page is clicked, we get the current record information from the model and fill out our form with the information of the current record. We check the validity of the form when the user makes changes to the form and clicks the update record button. If the form is valid, we save the form and redirect the user to the homepage with a message stating that the process was successful.

![Screenshot_4](https://github.com/tolgakb/DjangoCRMSample/assets/101968167/73f4894e-8d7b-4f12-bc07-59cefca84488)


