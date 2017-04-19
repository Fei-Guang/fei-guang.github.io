Basic Server Setup
To start off, we need to set the password of the PostgreSQL user (role) called "postgres"; we will not be able to access the server externally otherwise. As the local “postgres” Linux user, we are allowed to connect and manipulate the server using the psql command.

In a terminal, type:


sudo -u postgres psql postgres
this connects as a role with same name as the local user, i.e. "postgres", to the database called "postgres" (1st argument to psql).

Set a password for the "postgres" database role using the command:

\password postgres
and give your password when prompted. The password text will be hidden from the console for security purposes.

Type Control+D or \q to exit the posgreSQL prompt.

Create database

To create the first database, which we will call "mydb", simply type:


 sudo -u postgres createdb mydb