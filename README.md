# 111milRestService
A rest service example created at class

## HOW TO RUN IT

### Create a new database

mysql> create database db_example; -- Create the new database

### Update application.properties
In the sources folder, you create a resource file src/main/resources/application.properties

<pre class="prettyprint highlight" id="code-block-4"><code class="language-java" data-lang="java"><span class="pln">spring</span><span class="pun">.</span><span class="pln">jpa</span><span class="pun">.</span><span class="pln">hibernate</span><span class="pun">.</span><span class="pln">ddl</span><span class="pun">-</span><span class="kwd">auto</span><span class="pun">=</span><span class="pln">create
spring</span><span class="pun">.</span><span class="pln">datasource</span><span class="pun">.</span><span class="pln">url</span><span class="pun">=</span><span class="pln">jdbc</span><span class="pun">:</span><span class="pln">mysql</span><span class="pun">:</span><span class="com">//localhost:3306/db_example</span><span class="pln">
spring</span><span class="pun">.</span><span class="pln">datasource</span><span class="pun">.</span><span class="pln">username</span><span class="pun">=</span><span class="pln">MySqlUser
spring</span><span class="pun">.</span><span class="pln">datasource</span><span class="pun">.</span><span class="pln">password</span><span class="pun">=</span><span class="typ">ThePassword</span></code></pre>

Here, spring.jpa.hibernate.ddl-auto can be none, update, create, create-drop, refer to the Hibernate documentation for details.

- none This is the default for MySQL, no change to the database structure.
- update Hibernate changes the database according to the given Entity structures.
- create Creates the database every time, but don’t drop it when close.
- create-drop Creates the database then drops it when the SessionFactory closes.

### RUN

- mvn clean install
- java -jar target/gs-accessing-data-mysql-0.1.0.jar

### Test the application

localhost:8080/demo/all This gets all data localhost:8080/demo/add This adds one user to the data


This service was built using [Spring Guides](https://spring.io/guides/gs/accessing-data-mysql/).

