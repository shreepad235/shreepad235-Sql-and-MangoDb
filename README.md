


Let's connect mysql with python code

first again launch a new terminal.

execute below command
```
pip install mysql-connector-python
```

Create a file "demo.py" and paste the below snippet
```
import mysql.connector
# import mysql.connector
#create user 'user'@'%' identified by 'password'
mydb = mysql.connector.connect(
  host="localhost",
  user="abc",
  password="password"
)
print(mydb)
mycursor = mydb.cursor()
mycursor.execute("SHOW DATABASES")
for x in mycursor:
  print(x)
```

Now run the script
```
python demo.py
```
