# Reading Notes

## Code 401 - Advanced Software Development

### *Class 01 Reading*

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


### *Class 02 Reading*

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


### *Class 03 Reading*

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


### *Class 04 Reading*

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

### *Class 05 Reading*

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

### *Class 06 Reading*
**What does protocol mean?**
- A protocol is a set of rules that must be followed

**How does any web browser understand how to open any webpage?**
- Through a URL & Headers

**Name one thing a request object must have, and one thing a response object must have**
- Request must have a URL and the response must serve the body

**What is the difference between HTTP and REST?**
- HTTP is a communications protocol that transports messages over a network, Rest is a protocol to exchange any XML or JSON messages that can use HTTP to transport those messages. (credit to [Stack Overflow](https://stackoverflow.com/questions/2190836/what-is-the-difference-between-http-and-rest))

**Why is REST important?**
- For consistency! It's a collection of guidelines to give various servers a sense of consistency. If every API adopts the same standards, it makes it easier for clients to understand how to use your API!

<br><br>
<br><br>

### *Class 07 Reading*
**What code does the server actually run?**
-  The server runs handlers for different types of events.

**What Express/HTTP operations map to CRUD operations?**
- ``GET`` 
- ``POST``
- ``PUT``
- ``DELETE``

**What does res.send() do?**
- It sends a string response (res) in a format other than JSON. 

**What is the order of operations for the three categories of middleware (handler, application, route)?**
- Application: Run when the server recieves a request.
- Route: Runs when the server receives a request to a specific endpoint. 
- Handler: Runs when the server receives a specifc method request to a specified route.

**What is the parameter next used for?**
- Calling the next middleware in the chain or calling an error

<br><br>
<br><br>



### *Class 08 Reading*
**What is a benefit to using express.Router()?**
- Separation of concerns type of thinking. Using express.Router() we can house each major routing branch in a separate file 

**When I say that top-down order matters in Express, what does that mean?**
- The order of operations will run from top down, functions and other code that relies on different information will need to be run in such an order that the 'parent' code runs above the next block.

**Why do we use a model class (with create(), read(), etc.) instead of directly calling MongoDB operations (such as save(), find(), etc.) within our Express route handlers?**
- In order te ensure all data is collected before calling mongo then deliver a status code back to the user.
<br><br>
<br><br>






### *Class 09 Reading*
1. Describe a use-case where param middleware would come in handy.
- We can set middleware to run whenever a speicfied paramerter is present. It can be particularly useful for validating or formatting the req.params key-value before hitting a param

2. What are the two ways to add middleware in-between Mongoose and MongoDB interactions?
- app.param OR router.param - NO 'S'!

3. What is the difference between a join by reference and a virtual join?
- Join by reference: When the field is equal to an ID of another schema & mongoose replaces the ID with the full record
- Virtual join: Join by name instead of ID 

4. What do localField and foreignField mean?
- Having issues finding this one - looks like you use both together, possibly local stores it & foreign  keeps track of it? 

<br><br>
<br><br>

### *Class 10 Reading*
1. Why is authentication important?
- Restricting access to information

2. Why should we be careful about storing a user’s password?
- If not properly encrypted, a users private data & passwords could be leaked

3. What is the difference between hashing and encryption?
 - Encryption is a two-way function & the data can be decrypted with the proper key
 - Hashing is a one-way function that scrambles plain text to produce a unique message digest. There is no way to reveal the original password
 - (source: https://gcn.com/articles/2013/12/02/hashing-vs-encryption.aspx)

4. What is the difference between encryption and encoding?
- Encryption is for maintaining data confidentiality and requires the use of a key in order to return to plaintext.
- Encoding is for maintaining data usablity & can be reversed by employing the same algprithm that encoded the content (no key needed).
- (source: https://hackercombat.com/forum/network-security/whats-the-difference-between-encoding-encryption-and-hashing/)

5. What is a token used for?
- A token is used to make security decisions and to store tamper-proof information about some system entity

<br><br>
<br><br>

### *Class 11 Reading*

1. Come up with an application scenario where you would want to use a stack.
- Reversing a word

2. Come up with an application scenario where you would want to use a queue.
- A ticket buying app or pre-sale vendor thath puts users into an order

3. Why are pop, push, enqueue and dequeue always O(1)?
- It takes the same amount of time no matter how many Nodes (n) you have in the stack.

4. Why do stacks and queues not have traversal or searching operations?
- I think (keyword, think) that these data structures do have search functionality, Deapth-First & Breadth-First Searches. ([Source](https://www.cs.cmu.edu/~adamchik/15-121/lectures/Stacks%20and%20Queues/Stacks%20and%20Queues.html))

<br><br>
<br><br>

### *Class 12 Reading*

1. What’s a benefit of using OAuth instead of your own basic authentication?
-  It standardizes how independent web applications can share user data without sharing user passwords. Instead of a password, your site recieves less sensitive information like your name, email, profile picture, etc.

2. Write the following steps in the correct order:
* Make a request to a third-party API endpoint
* Redirect to a third party authentication endpoint
* Ask the client if they want to sign in via a third party
* Receive authroization code
* Register your application to get a client_id and client_secret
* Receive access token
* Make a request to the access token endpoint

3. What can you do with an authorization code?
- Read data from the user’s account

4. What can you do with an access token?
- Sign in a user & read that user's data

<br><br>
<br><br>

### *Class 13 Reading*

1. When is Basic Authorization used vs. Bearer Authorization?
- Basic takes in a username and client secret, bearer takes in a token

2. What does the JSON Web Token package do?
- Defines a compact and self-contained way to securely transmit information between two systems (servers, clients, etc.) as a JSON object. 

3. What considerations should we make when creating and storing a SECRET?
- They are not as secure as a standard encrypted string, so there is still a risk that the encrypted content could be hacked into. Due to this, do not to put any sensitive user data into the token. 


<br><br>
<br><br>

### *Class 14 Reading*
1. Why is access control important? Describe an application that would need access control.
- Access control is important to keep the integrity of some data/apps at a certain level. An example would be any program used by HR in company - only a manager would be able to see and adjust thier employees salary, where as the employee may only be able to input their hours.

2. What is a role used for?
- Defining what the user capabilities will be able and what they'll be able to do on a site


3. Why is role based access control more scalable than discretionary or mandatory access control?
- In both the mandatory & discresionary access control situations, it seems that a single authority has to allocate access for certain users - when it reaches millions of users, this could be difficult, if not impossible, to manage. If every user is automatically assigned to a role and that role is clear on what access they need, it can be automated & simplified only needing an adjustment if they change roles.


<br><br>
<br><br>

### *Class 15 Reading*

1. What is a leaf node? Why is it important to be able to find leaf nodes?
- The leaf node is the last node in a tree with no attached edges - when traversing a tree, once it hits a leaf and both left and right return null, it will end the execution of the method.

2. Describe the differences between pre-order, in-order, and post-order traversal. Why are they called pre, in, and post order?
- PRE: means that the root has to be looked at first/top to bottom
- POST: this means that the root is looked at last/bottom to top
- IN: reads the tree from left to right

3. What is the height of a fully balanced (each non-leaf node has two children) tree? What is this used for?
- log(n) , used for searching. If a tree is balanced, it is easier to say for sure how the big O is going to look. If unbalanced, worse case, one side could be O(1) where the other is o(n)

4. How are stacks and queues used in relation to trees?
- They are used to hold the place of the traversal as it goes through the tree - as if reaches a leaf, values are popped or dequeued onto the return

<br><br>
<br><br>

### *Class 16 Reading*
1. Given the examples of front-end events such as button click, window resize, form submit, etc, what are some examples of back-end events?
- Getting data from a database, setting a timeout, reading a file, threads, events, event queue, and event loop.


2. Why are events sometimes better than asynchronous actions with callbacks?
- Asynchronous actionst can take an unknown amount of time and we don’t want our application to be on pause,

3. What does an EventEmitter instance do?
- The EventEmitter class allows us to both raise new events and to listen to events that have been raised.

4. When is a program’s call stack, event queue, and event loop active?
- When we call ``emit`` in our code


<br><br>
<br><br>

### *Class 17 Reading*

1. What do the layers in the OSI and TCP/IP models represent?
- A series of rules or the fundamental pieces of the process of connecting 2 systems to ensure security & that each application knows what to do

2. What is the benefit of transforming data into packets?
- They're easier to send over the internet

3. UDP is often referrered to as a connectionless protocol. Why is this?
- When transferring data it doesn’t establish a strong secure connection between the sending server and the receiving server

4. Can a socket server application have multiple socket connections? Can a socket connection application be connected to multiple socket servers? Can an application be both a socket server and a socket connection?
- Yes
- No
- Yes??
 
<br><br>
<br><br>

### *Class 18 Reading*
1. What does it mean that web sockets are bidirectional? Why is this useful?
- The sockets are ever-connected & two-way. Web sockets remain connected during their lifetime, and they are well suited for real-time data transfer over the web.

2. Does socket.io use HTTP? Why?
- Yes, because they are geared at creating web sockets, they can take advantage of some of the HTTP protocol benefits. socket.io connects to both HTTP & TCP. The HTTP layer is to ensure that the connection is kept active and authenticated.

3. What happens when a client emits an event? What happens when a server emits an event?
- The client can emit an event to the server, and the server can emit an event to other connected clients/apps.

<br><br>
<br><br>

### *Class 19 Reading*
1. What is the main benefit of a message queue server?
- Connects clients with the data they need. 

2. Why might we want to initiate messages from an HTTP request?
- When the event is reciceved iva /post, the action can then be triggered.

3. Is the Message Queue Server a socket.io client, a socket.io server, or an api server?
- I believe this is a socket.io server, reiceiving messages from the api server, then serving messages to the socket client

<br><br>
<br><br>

### *Class 21 Reading*
1. What is the benefit of breaking up HTML webpage content into components?
- Makes it easier for continuity between pages

2. What is JSX? Why is it useful?
- Short for JavaScript XML - it allows for JavaScript and HTML to be seemlessly mixed together 

3. What can cause a render (or re-render) of a component?
- A structural change, changing a component’s state variable

4. When a render happens, how is the DOM affected
-  The components appear on the page & within the DOM 

5. What is one thing a framework does that a library doesn’t do?
- When you call a method from a library, you are in control. But with a framework, the control is inverted: the framework calls you. (src:https://www.programcreek.com/2011/09/what-is-the-difference-between-a-java-library-and-a-framework/#:~:text=The%20key%20difference%20between%20a,a%20collection%20of%20class%20definitions. )

<br><br>
<br><br>

### *Class 22 Reading*
1. Describe a case where snapshot testing would be useful, and describe another case where it would be ineffective.
- EFFECTIVE: For a fully developed UI page that you want to ensure does not change throughout development
- INEFFECTIVE: During development when the UI is constantly changing

2. What is the difference between full mount and shallow mount?
- Full mounting allows you render the entire component as well as any children components. Shallow mounting minimized the render of any imported components, and instead focuses on fully rendering the current component only.

3. What does npm run build do?
-  It lets you perform any necessary building/prep tasks for your project, prior to it being used in another project.
 By running npm run build, it optimizes your React code for production deployment. Once run, this script creates a seemingly static website with just an index.html

<br><br>
<br><br>

### *Class 23 Reading*
1. Why might you want to create a FormInput component?
- To hold form data

2. Can a parent component access the state of a child component?
- Yes ( I think? ) - by using props, I see that the  child component doesn't have tp wrry about the state, but I cannot tell if the parent can access the child's state

3. What can be passed along in a prop variable?
- Static variable data or entire functions

<br><br>
<br><br>

### *Class 24 Reading*
1. Why do we not need more .html pages in a multi-page React app?
- Instead of adding additional pages, we'll be using ```react-router-dom``` which allows us to essentially build a switch statement of what components are rendered based on the browser URL.

2. If we wanted a component to show up on every page, where would we put it and why?
>Outside the <BrowserRouter/>
>Inside the <BrowserRouter />, outside a <Route />
>Inside a <Route />
- Inside a <Route />

3. What does props.children contain?
- It is used to display whatever you include between the opening and closing tags when invoking a component.

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
- How? Start with an issue or solution to be explored, as either how or why 5 times digging to get to the root. 