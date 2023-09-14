Task2 : CRUD Operation CRUD Operations – What is CRUD? Despite being commonly pronounced /krʌd/, CRUD is not a word. It’s an abbreviation that stands for Create, Read, Update, and Delete or Destroy.

CRUD refers to the four basic operations a software application should be able to perform – Create, Read, Update, and Delete.

In such apps, users must be able to create data, have access to the data in the UI by reading the data, update or edit the data, and delete the data.

In full-fledged applications, CRUD apps consist of 3 parts: an API (or server), a database, and a user interface (UI).

The API contains the code and methods, the database stores and helps the user retrieve the information, while the user interface helps users interact with the app.

You can make a CRUD app with any of the programming languages out there. And the app doesn’t have to be full stack – you can make a CRUD app with client-side JavaScript.

In fact, the app with which I will be showing you how create, read, update and delete operations work is made with client-side JavaScript.

Each letter in the CRUD acronym has a corresponding HTTP request method.

CRUD OPERATION HTTP REQUEST METHOD Create POST Read GET Update PUT or PATCH Delete DELETE What is the CREATE Operation and How Does it Work? In CRUD, the create operation does what the name implies. It means creating an entry. This entry could be an account, user information, a post, or a task.

As I pointed out earlier, the HTTP protocol that implements a CREATE operation is the POST method.

In a SQL database, to create is to INSERT. In a NoSQL database like MongoDB, you create with the insert() method.

In a user interface, this GIF below shows how the CREATE operation works: create-op

What is the READ Operation and How Does it Work? The READ operation means getting access to the inputs or entries in the UI. That is, seeing it. Again, the entry could be anything from user information to social media posts, and others.

This access could mean the user getting access to the created entries right after creating them, or searching for them. Searching is implemented to allow the user to filter out the entries they don’t need.

The HTTP protocol that implements a READ operation is the GET method.

In a SQL database, to read is to SELECT an entry. In a NoSQL database like MongoDB, you read with the find() or findById() method. read-operation

What is the UPDATE Operation and How Does it Work? UPDATE is the operation that allows you to modify existing data. That is, editing the data.

Unlike READ, the UPDATE operation alters the existing data by making changes to it.

PUT and PATCH are the HTTP protocols with which you can implement an UPDATE operation, depending on what you need.

PUT should be used when you want the entire entry updated, and PATCH if you don’t want the entire entry to be modified.

In a SQL database, you use UPDATE to update an entry. In a NoSQL database like MongoDB, you can implement an update feature with the findByIdAndUpdate() method.

In a user interface, this GIF below shows how the UPDATE operation works: update-op

What is the DELETE Operation and How Does it Work? To delete is to get rid of an entry from the UI and the database.

DELETE is the HTTP protocol for implementing a DELETE operation.

In a SQL database, DELETE is used to delete an entry. In a NoSQL database like MongoDB, you can implement delete with the findByIdAndDelete() method. delete-op
