### Conceptual Exercise

Answer the following questions below:

- What is PostgreSQL?
       PostgreSQL is a free and open-source relational database management system that uses and extends SQL language
       combined with many features that safely store and scale the lost complicated data workloads.


- What is the difference between SQL and PostgreSQL?
        SQL server is a database management system which is mainly used for e-commerce and providing different data warehousing solutions. PostgreSQL is an advanced version of SQL which provides support to different functions of SQL like foreign keys, subqueries, triggers, and different user-defined types and functions.


- In `psql`, how do you connect to a database?
        You connect to a database by using the command '\c DATABASE_NAME'.


- What is the difference between `HAVING` and `WHERE`?
        HAVING is used for filtering when the data is grouped. WHERE is used to filter data without grouping.
        
- What is the difference between an `INNER` and `OUTER` join?
        INNER join results with the intersection of two tables, meaning it outputs only the fields which are common in both the tables.
        OUTER join results with the union of two tables, meaning it outputs all the fields in the both the tables.

- What is the difference between a `LEFT OUTER` and `RIGHT OUTER` join?
        The key difference between a left outer join, and a right outer join is that in a left outer join it's the table in the FROM clause whose all rows are returned. Whereas, in a right outer join we are returning all rows from the table specified in the join clause.

- What is an ORM? What do they do?
        An object-relational mapper (ORM) is a code library that automates the transfer of data stored in relational database tables into objects that are more commonly used in application code.

- What are some differences between making HTTP requests using AJAX 
  and from the server side using a library like `requests`?
        *)Client-side HTTP requests are done using AJAX through a browser whereas Server-side HTTP requests are done using the requests library through curl or a backend program.
        *)AJAX request is used to fetch data from a database. Server-side request using libaries is used to deliver the app which includes HTML,CSS,JS etc to the client from the server 


- What is CSRF? What is the purpose of the CSRF token?
        Cross-Site Request Forgery (CSRF) is an attack that forces authenticated users to submit a request to a Web application against which they are currently authenticated. CSRF attacks exploit the trust a Web application has in an authenticated user.  
      CSRF Token or a Synchronizer Token, works as follows:
          The client requests an HTML page that contains a form.
          The server includes two tokens in the response. One token is sent as a cookie. The other is placed in a hidden form field. The tokens are generated randomly so that an adversary cannot guess the values.
          When the client submits the form, it must send both tokens back to the server. The client sends the cookie token as a cookie, and it sends the form token inside the form data. (A browser client automatically does this when the user submits the form.)
          If a request does not include both tokens, the server disallows the request.

- What is the purpose of `form.hidden_tag()`?
          The form. hidden_tag() template argument generates a hidden field that includes a token that is used to protect the form against CSRF attacks. All you need to do to have the form protected is include this hidden field and have the SECRET_KEY variable defined in the Flask configuration.