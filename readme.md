json-server --watch db.json

http://localhost:3000/employees/2
http://localhost:3000/employees?first_name=Jesse
http://localhost:3000/employees?q=Nate
http://localhost:3000/employees?q=@hotmail.com

PostMan
delete
-----------------------------------------------------------------
http://localhost:3000/employees/2 

deletes from the actual db.json file
-----------------------------------------------------------------

post
-----------------------------------------------------------------
http://localhost:3000/employees

{
  "id": 2,
  "first_name": "Nate",
  "last_name": "Soldat",
  "email": "nate@hotmail.com"
}
body----
raw / change text to JSON (application/json) this will update the headers
-----------------------------------------------------------------

put
-----------------------------------------------------------------
http://localhost:3000/employees/2

{  
  "first_name": "Nate",
  "last_name": "Soldat",
  "email": "nate@hotmail.com",
  "work": "The Beltline"
}

body-------
raw / change text to JSON (application/json) this will update the headers
-----------------------------------------------------------------

faker.js
https://github.com/marak/Faker.js/
npm install faker --save

after making your js file with the generateEmployees function

json-server employees.js


