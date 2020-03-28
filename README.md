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

<br><br>
<br><br>


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

<br><br>
<br><br>

*Class 05 Reading*

**What is a data structure?**
-  A data structure is a collection of data values, the relationships among them, and the functions or operations that can be applied to the data. 
[Wikipedia page definition](https://en.wikipedia.org/wiki/Data_structure) 
* Examples include: variables, arrays, hashes, and objects

**How is a Linked List different from an array?**
- Arrays are more rigid, more difficult to change & memory managment
- Arrays are static data structures where linked lists are dynamic

**What is one benefit a Linked List has over an array?**
- It is simpler to change a linked list than it is to change an array

**What data does a Node hold in a doubly Linked List?**
- Sequentially linked records

**What would you use to implement a Linked List data type? (object, function, class, variable…?)**
- I'm not enitrely sure on this one, I believe we'd use a class to create a constructor for adding items to the linked list, but I feel like that's wrong. Looking forward to learning more about it! 


<br><br>
<br><br>

### Engineering Topics

#### Solving Problems
- The most common mistake while watching someone try to solve a programming problem is they try to start writing code as soon as possible. You must resist this urge
1. Read the problem completely twice.
-  A good test of this is whether or not you can explain the problem to someone else. 

2. Solve the problem manually with 3 sets of sample data.
- Solve the problem manually first, so that you know what you are going to automate, otherwise you are just slinging code around.

3. Optimize the manual steps.
- Figure out if there is another way you can solve the problem easier, or if there are some steps you can cut our or simplify.

4. Write the manual steps as comments or pseudo-code.
- Capture all the steps we created and now either put them into our editor as comments or write them as psuedo-code that we can translate to real code

5. Replace the comments or pseudo-code with real code.
- All we do here is take each comment and convert it into a real line of code.

6. Optimize the real code.
- It's important having good names for your variables and methods is for helping the person evaluating your code to understand what you were trying to do

* As much as 70% of our time should be spent in steps 1-3.

#### Act like you make $1000/hr
- If you let it, your world and the people around you will take all your time. Your time is not unlike your paycheck; if you don’t budget for things, you’ll have nothing left over by the end of the month

- Extremely successful people don’t tolerate busywork or distraction. They have crystal clear vision on their goals, and do what they need to do to get there, every single day.

#### How to think like a programmer
1. Understand 
- Know exactly what is being asked.
2. Plan
- Don’t dive right into solving without a plan (and somehow hope you can muddle your way through). Plan your solution!
3. Divide
- **Do not try to solve one big problem. You will cry.**
- Break up your problem, solve each sub-problem one by one. Begin with the simplest. Simplest means you know the answer (or are closer to that answer).
4. Stuck?
- Debug: Go step by step through your solution trying to find where you went wrong. Programmers call this debugging (in fact, this is all a debugger does).

- Practice 

#### The 5 Whys & Hows
- The five whys and five hows constitute a questioning process designed to drill down into the details of a problem or a solution and peel away the layers of symptoms.
- Why? To explore the root of the problem & really dig in
- How? Start with an issue or solution to be explored, as either how or why 5 times digging to get to the root