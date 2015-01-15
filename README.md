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




