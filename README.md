<h2>Dan's Frappuccino Paradise Shop Application </h2>
<hr>
This project creates a functional web-app for a frappuccino shop.  This includes
menu access, online ordering, in-house ordering, inventory control,
and payroll management.
<h3>Workspace Layout</h3>
<hr>
Dan's Frappuccino Paradise Shop Web App will be stored on this repository.

Any documentation and resources for this project will be kept in the "docs" folder.
This includes use case diagrams, the project plan, and project requirements.  More may 
be added as the project progresses.

The code for the application and server will be kept in the "app" folder.
<br>
<h3>Version-Control Procedures</h3>
<hr>
Collaborators must fork the repository found at Zachary-Harrison/cs3450-group10.
The forked repository must then be cloned.  After completing any work, collaborators
should submit a pull request so that all progress is documented and issues may be discussed.
Commit messages should be clear to assist in task control.
<h3>Tool Stack Description and Setup Procedure</h3>
<hr>
Django - Simple server, database, and encryption capabilities

Python - Most team members are familiar with Python and it is very effective for background processes.

JavaScript - This will assist in making the site aesthetically pleasing and provide
some additional functionality.
<h3>Build Instructions</h3>
<hr>
Clone the project in gitbash.

> bash $ git clone https://github.com/Zachary-Harrison/cs3450-group10

Install Django via pip3

> bash $ sudo pip3 install django

Navigate to the project sub-folder. 

> bash $ cd app/cs3450_group10

Run the server using the following command.

> bash $ python manage.py runserver 3000

In a web browser, navigate to http://localhost:3000/shop_app to view the app.


<h3>Unit Testing Instructions</h3>
<hr>
    

<h3>System Testing Instructions</h3>
<hr>
<h4>Test if server is on correct port and open</h4>

        > bash $ sudo ss -tnlp || grep -m 1 -w -F '127.0.0.1:3000'

    This should result in one of the lines looking like so:

    "LISTEN              0                   10                                    127.0.0.1:3000                                   0.0.0.0:*                  users:(("python3",pid=104387,fd=4))"

    If this fails try:

        > bash $ sudo netstat -tnlp || grep -m 1 -w -F '127.0.0.1:3000'

    This should be the result:

        "tcp        0      0 127.0.0.1:3000          0.0.0.0:*               LISTEN      104387/python3"

<h4>Check if server is serving files</h4>

    Open prefered web browser and type this into the search bar:

    "http://127.0.0.1:3000/shop_app/"

    Should result in the shop page.
<h3>Other Development Notes</h3>
<hr>
