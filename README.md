Mochammad Ezar Yudha
2206046746
CS KKI

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


