# s15_Chinni_data_lecture_notes

##Lecture 1

Big data is found in:

a) Social Netwoks

b) Data Analytics
    Most of the  machine learning will be done here. For example if a company needs to find out the interest of the customer with his most recent purchases and offer him with the best products.
    
c) Storage - NoSql
     NoSql is not very good at handling the Non-Orbitrary queries. 
     Documents, Graphs, Key-Value, colomar store. 
     Twitter uses UTF8 for saving their tweets. 
     It is very difficult to collect the data and store as the data is non-uniform and it may have differnet characters and     Images. 

d) Data LifeCycle. (steps)
     ->Colletion of the generating data.(Data is collected up on knowing what has to be collected called as question apart of it one more content is Curation another aspect of Curation is Triag(prioritization of the situation)and in the end persistance of the data)
     * Clean up 
     * Storage. 
     * Processing/Analysis 
     * query/Visualization/Act.(Gives the new question with the received answer)
    
    Http request response Cycle. 
     
##Lecture2:

Distributed control systems which will help others also to edit and maintain the version control. 
###GitHub MarkDown
Markup language: This is like the normal HTML Markup languge it uses plain text to create rich test.(bullets, tables etc).  
* GitHub Lable Markdown
* standard Markdown
   * Plain text formatting , creating tables, formatting, Images can also be added, There are list (ordered and unordered), create links, block of codes.
   * Creating headers: There are different types of headers, these can be created by using hash pounds before heading. 
   * Italics and bold text can also be created. 
   * we can use astric and numbers before the lines with two spaces. 
   * To provide a link [Google homepage](www.google.com).
   * Codeblocks and syntax use three back-ticks in the starting and the ending of the code. It will Automatically adds the colors to the words according to the language. 
   * Tables-
   * To create horizantal lines use 3 Hyphens, Asterisks or underscores.  

Web browser will send a request to the webserver to get a particular page from a website. ex: www.ebay.com/product/20, this will use GET, POST, Delete, and Put. Delete should be done with care so that people cannot send delete request and delete the data. The webserver will ask the handler(Saperate entity ex: Apache webserver etc) about the request.The handler will point out the HMTL file in the disk and then send it to the browser now browser will get additional data from the webserver if there are any further links in the received HTML Page.  Rest is an Architecture for buling server based request.Respresentation of state transfer(REST)  
* Resources called URI(Relationship is subset of URI-URL)(URL has a limit of 1024bits)
* CRUD(Create Read Update and Desination)
* GET-Read operation and get back the current state of the Resource. 
* POST- Creating a new Resouce(Data which helps to create new user)
* PUT- Update. (Update the existing user for the particular data)
* DELETE - Destroy the user.  

While creating a webservice we need to think of:
* database to use and how to get the ID for the data. 
* Input to be used
* What output ?
* Errors. 

##Lecture 3:

* Get: Retrive a list of all users
  * GET/api/2.0/users/0 - Retrive the details of users 0.
  * POST/api/2.0/users- Create a new user. 
  * PUT/api/2.0/users/0 - Update user 0 
  * DELETE/apt/2.0/users/0 - Delete user 0.
  * GET/api/2.0/serach?w=tattersail - Perform a serach with the tattersail.


Each operation may produce a result with Restful services, JSON format is king. POst and PUT methods typically send data in JSON format. FOR Get the data may appear as uery params. 

Other formats are possible like HTML , XML are typical. ruest needs to be authenticated this authentication data appears in HTTP Headers. 

###How operations on two resources are handled?

* One approach is GET/api/2.0/posts/0/comments/2 - Get First comment on post 0.
* POST/api/2.0/posts/0/comments- Create a new comment on post 0.
* 
Alternative Approace.

* while performing an operation on one resource, you 

Issues:

* Security: how to authenticate.
* Identity: How Id's are assigned to resouces. 
* Failure: How to handle the failure situations
* persistence: How are resouces Stored. 
* (respec)
Technologies used: 
* sinatra
* Rspec
* Typhoeus
* Node
* Express


 
##Lecture 4:

#####Git Version controlling:

Master is created during the first commit when ever a new commit is made a Head is added to the master. If some of tries to fix the bugs for a given code then the head and the master will be pointed to the current node. Git merge Master is used to make sure that the other person who is using the same code will see the changes for this just say Git merge sort(This works when there are two parents.)

#####Git Hub workflow

Master->branch ->pullreuest. Master represents production ready code all the pusing should be done on branches. Pull reuest to add the code to the available branch If you have collabrated access. if there is no collabrated access use fork. Fork is an exact copy of the repository. 

##Lecture 7:

React frame work better than angular. sublime(ide) 

##Lecture 8:

Myfirst git In angular one can assign variables and methods to this in a controller we cannot allocate this with a number. 

Consumer key and secret key. and get the token access consumer key and secret key. 
developers documentation 

##Lecture 10:

Getting data from twitter take two: OAuth is the secuirty protocol that is used to take care of who is looking in what kind of data. call back url is used to give an external site the access of what is happening in some ones twitter account. 

####Accessing twitter data via the Rest:
    It should have a single JSON object inside with the consumer key, accesskey details. use rbenv to manage ruby on your  machine. __File__ is the current file that is executing. JQ is the tool required for json files. 

##Lecture 12: 

Shard the database which means multiple instances of the database server. Different databases each with its filesystems. Sharding should be done very carfully otherwise its difficult to get back the server live it takes time to troubleshoot. 


##Lecture 13:

Couch DB:  
 * Document Model. 
 * It stores Documents.
 * Each document contains every thing that is need for an application. 
 * CAP Therom:
 * Consistency: All clients see the same data even in the presence of concurrent updates.
 * Availability: All clients are available at all time for reading and writing. 
 * Partition Tolerance: Database can be split across multiple servers. The Cap theorm says pick any two of these features. 
 * Couch db will choose Availability and partition tolerance.(even many nosql systems does this).
 * CouchDB makes use of a B-tree storage engine, Automatic sorting, seraches , insertion, and deletion occur in deletion time. 
 * Employs MapReduce over this B-tree to compute views of the data allowing for parallel and incremental computation. 
 * No Locking: CouchDB does not requiree locks for concurrent access to its documents. 
 * It will return the latese version of the document and a new version of the document can be written while a read occurs the next read will return the new updated document. 
 * Validation function can be written in Js for a particular class of document. 
 * Incremental Replication: synchronization of data between servers can be done when ever is necessary. 
 * once replication is doen all the copies are independent. 
 * Merge Conflicts: Each document will have a version id and a separate id. 
 
##NEOJ

* This is the graph database where the nodes are the data and the edges are the relation between them. 
* We can use findallpaths() to find all the incoming and out going paths from a node to b node. 
* shortestpath() finds the shortest path between two different nodes. 
* Gremlin is specific language for travesing graph or cypher can be used. Lucene for full text search.
* Aggretated orientation database

##Hbase:
* Hbase run over hadoop which has map reduce and hdfs file system. hbase run over hdfs file system which is coloumn based.
* Hdfs is a batch processing. Column families and each has multiple columns. 
* Each cell value of the table has a timestamp to retrive based on the timestamp. 
* table->collection of roles
* row-> collection of column families
* column Family -> collection of columns. 
* Data is de-normalized
* Zookeeper will keep track of all the nodes and information of the meta file.
* Zookeeper keeps the location of the system table .META. 
* If there is too much data in one region it will trigger a split and transfer the data. 
* When to use Hbase is large amount of data in client.
* Horizantally scalable - Automatic Sharding. 


