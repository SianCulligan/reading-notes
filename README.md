# Reading Notes

**Code 401 - Advanced Software Development**

*Class 01 Reading*

**Why would you want to run JavaScript code outside of a browser?**
- Running JavaScript outside a browser means you are using node. js to execute your JavaScript code - this allows us to use JavaScript without using an HTML page to run functions. 

**What is the difference between a module and a package?**
- A package is an extension of a module - while a module is a single JavaScript file that needs to be called in another file, a package is a directory containing complex chunks of code that can be shared with other developers.

**What is one benefit of Test Driven Development?**
- By planning out the input format & expected outputs before development,  it can help prevent uncertainty during the process & create almost a set of guiding principles while writing code.

**What is one potential downside of Test Driven Development?**
- If we're not starting from scratch, I can see this being difficult to write for legacy code. Also, maintenance as the codebase changes.

**What does the node package manager do?**
- It allows us to use packages created and shared by independent developers




*Class 02 Reading*

**What is one benefit of JavaScript not enforcing type?**
- You can change the type on the fly, as needed.

**What is one downside of JavaScript not enforcing type?**
- You can get into situations where your variable is not containing the type of data that it should. These kinds of errors can become very hard to track and solve in large code bases.

**Should the parameters of a function be changed when the function returns? Why or why not?**
- Depends on the situation, if we're able to change parameters, we can re-use functions to do different tasks.

**Describe a type of data that has rules, aside from the given examples of Number, Integer and Float. What are the rules the data should follow?**
- A boolean, which represents only one of two values: true or false.



<br><br>
<br><br>


*Class 03 Reading*

**Why would a developer choose to make data models?**
- Provides structure and consensus for end project. Almost as if to establish best practices, but for software.

**What purpose do CRUD operations serve?**
- Provides a mempoable framework, these operations link to a series of commands.

**What kind of database is Postgres? What kind of database is MongoDB?**
- Postgres os a SQL database, more rigid and stuctured, MongoDB is a noSql database that can use a variety of languages to access data

**What is Mongoose and why do we need it?**
- It is the most popular, NoSQL database that allows flexibility with data as an app evolves/ 

**Define three related pieces of data in a possible application. An example for a store application might be Product, Category and Department. Describe the contraints and rules on each piece of data and how you would relate these pieces to each other. For example, each Product has a Category and belongs in a Department.**
- Customer: Has both a birthday and hair color
- Birthday: Belongs to the customer, but does not have a hair color 
- Hair Color: Attribute of the customer, no birthday


<br><br>
<br><br>


*Class 04 Reading*

**What makes an interface useful?**
- It standarizes and simplifies complex operations 

**Why is middleware called middleware?**
- It's software that exists between two other software, or. more literally, middle software. 

**Fundamentally, what does it mean to have a mock of something? Why is this useful?**
-  Mocks are fake methods  with pre-programmed behavior as well as pre-programmed expectations. This is useful while in the tesing phase of developement.

**What does it mean to have a mock database?**
- Creating a fake database with the samesame structure, data models, and commands but it only exists for the lifetime of the test.