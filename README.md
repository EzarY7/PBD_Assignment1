Mochammad Ezar Yudha
2206046746
CS KKI

Assignment 2

1. How do you implement the tasks in the checklist? Explain in a step-by-step manner (not just copy-paste from the tutorial).
>> I first initilize a git repository that will be used as the base of the django project.
> This is done by creating a git repository on github, then creating a local repository and performing add, push, and commit so that the changes can be stored on the central repository on github.

>>Then, I activate a virtual environment

>>Once the virtual environment is set up, I set up and install dependencies for the django project and create the django project

>>The django project utilizes the MVT structure which stands for model, view, and template.

>>The next step is to create the an application called main.

>>Once the application is created, I can start to modify the template in the form of an html file.

>>Next, I can modify the model which essentially serves as a database schema. This contains the item along with its attributes.

>>To keep track of the state of the database schema, I apply migrations.

>>Next, I connect the views to the template. Views acts as a bridge to connect the data retrieved from the model to the template. I do this by creating a function in the views.py file.

>>Once I've implemented the MVT structure, I can configure the url routing so that the application can be accessed through the browser.

>>Next, I can use testing to see if the url can be accessed as intended.

>>Finally, I can perform add, push, and commit to save the changes to the central repository.

2.
<img src="Diagram/PBDDiagram1.png">



3.A virtual environment is used to isolate dependencies and libraries of different projects to prevent errors in the case that an updated library causes clashes with previous versions. We can create a django project without the use of a virtual environment but it is not the best practice.

4.MVC stands for Model, View, and Controller. The model handles all of the data-logic that the user can work with. The View handles the UI logic for the application. Controllers act as an interface between the model and view and processes the incoming requests to create the final output.

MVT stands for Model, View, and Template. The model serves as a database schema which contains the item along with its attributes. The Template serves as an interface for the application. The View serves as a bridge to connect the data retrieved from the model to the template.

MVVM stands for Model, View, and ViewModel. Model hands the data logic. View serves as an interface of the application. ViewModel links the view to the model by data binding.






Assignment 3

1.What is the difference between POST form and GET form in Django?
In post form, data submitted is included in the HTTP request body rather than in the URL. This form is suitable when transmitting sensitive data such as login information. On the other hand, data submitted in get form is appended to the URL as query parameters, this may cause security risks.

2.What are the main differences between XML, JSON, and HTML in the context of data delivery?
XML (Extensible Markup Language) is self-descriptive and is used to represent data hierarchically using tags. JSON (JavaScript Object Notation) represents data using key-value pairs. HTML (The HyperText Markup Language) uses tags to structure content on webpages.

3.Why is JSON often used in data exchange between modern web applications?
JSON's readibility is the one of the main reasons why its use so widespead among modern web applications. The representation of data as key-value pairs allow developers to easily understand the structure.

4.Explain how you implemented the checklist above step-by-step (not just following the tutorial).

Create a form input to add a model object to the previous app.
I created a new file called forms.py and added code to accept new data as input. This code consists of a class that contains the variable "fields", which is used to select the attributes from the model.

Add 5 views to view the added objects in HTML, XML, JSON, XML by ID, and JSON by ID formats.
I created 5 different functions, one for each format, in the views.py file. Each of them will accept Item objects and return the data in their respective formats.

Create URL routing for each of the views added in point 2.
I added the URL paths for each format to the urlpatterns list in urls.py.

Assignment 4

1.What is UserCreationForm in Django? Explain its advantages and disadvantages.
UserCreationForm is a built in tool in django which allows the creation of user accounts. Its simple to use and ensures security and validation from the user. It is limited by how basic it looks visually and it is less flexible due to the lack of control we have when compared to buulding a registration form from scratch.

2.What is the difference between authentication and authorization in Django application? Why are both important?
Authentication is the process of verifying the user's indentity wheras authorization is the process of determining what that user is able to access. They are both important in order to ensure security and privacy by reducing the amount of unauthorized user's accessing data.

3.What are cookies in website? How does Django use cookies to manage user session data?
Cookies are client-side files temporarily stored on the system which includes things such as login-status and browsing activities. Cookies are used to improve the user's experience as well as to analyze the user's behavior. One way that Django utilizes this is by allowing user's to see the time of their last log-in.

4.Are cookies secure to use? Is there potential risk to be aware of?
Cookies are generally safe to use. However, there are potential risks that developers need to consider. One such risk is the case where an attacker steals a user's cookies and therefore is able to impersonate the user. Developer's also need to ensure that sensitive data stored in cookies are encrypted to add extra security.

5.Explain how you implemented the checklist above step-by-step (not just following the tutorial).

Implement registration, login, and logout functions to allow users to access the previous application.
I first imported UserCreationForm which is a built in form in django which simplifies te creation of a registration form. I then created the form function in views.py and added an html file for the registration form. I then added the url path for the registration form. I then imported built in functions for login and logout and followed a similar procedure as with the registration form.

Create two user accounts with three dummy data entries for each account using the model previously created in the application.
I simply created 2 accounts and added 3 entries for each.

Connect Item model with User
I modified the model to create a relationship that associates each item to one user. I then modified the show main function so that the website displays items associated with the user. I then applied migrations to save the changes made to the model.

Display the information of the logged-in user, such as their username, and applying cookies, such as last login, on the main application page.
I modified the 'name' variable in the model so that it shows the user's name. I then modified the views.py file to include information on the user's last login.

