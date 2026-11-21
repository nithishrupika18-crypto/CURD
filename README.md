# EX.No: 03 DEVELOP A DJANGO-BASED CRUD APPLICATION
## Date:
## AIM

To develop a Django-based web application that performs CRUD (Create, Read, Update, and Delete) operations on student records.

## ALGORITHM

1. Create a Django project and an application.
2. Define the `Student` model with the required fields (Name and Email).
3. Run migrations to create the database table.
4. Configure URL routing for Home, Add, Update, and Delete operations.
5. Create the `home()` view to retrieve and display all student records.
6. Create the `add()` view to insert a new student record into the database.
7. Create the `update()` view to modify an existing student record using its ID.
8. Create the `delete()` view to remove a student record using its ID.
9. Design the HTML page with separate forms/buttons for Add, View, Update, and Delete operations.
10. Run the Django development server and perform all CRUD operations through the web browser.

## PROGRAM
```
<html>
    <head>
        <title>calculate</title>
        <style>
            body {
             background-color:cyan;
            }
        
        form{
            text-align:center;

        }
        label{
            font-weight:bold;
            font-size:20px;
            display:inline-block;
            width:150px;
            text-align:right;

        }
        input{
            width:250px;
            height:30px;
            box-sizing:border-box;
        }
        label {
            margin-bottom:8px;
        }
        input{
            margin-bottom:8px;
        }
        button{
            margin-top:15px;
        }
        .title{
            text-decoration:underline double;
        }
        label {
            white-space:nowrap;
        }
        </style>
        
    </head>
    <body>
        <form method="POST">
             {% csrf_token %}
             <h1 class="title">churn rate calculation</h1>
             <label><b>customer at start:</b></label>
        <input type="number" name="cstart"><br>
        <label><b>customer lost:</b></label>
        <input type="number" name="clost"> <br>
        <button>calculate</button>
        <h3>cstart value is: {{st}} </h3>
        <h3>clost value is :{{lt}} </h3>
        <h3>churn_rate is {{result}}%: </h3>
       </form>
    </body>
</html>
```


## OUTPUT

![alt text](<Screenshot 2026-11-21 180319.png>)

## RESULT

A Django-based CRUD web application was successfully developed to perform Create, Read, Update, and Delete operations on student records using SQLite as the backend database.


