# 111milRestService
A rest service example created at class


## Create a new database

mysql> create database db_example; -- Create the new database

## Update application.properties
In the sources folder, you create a resource file src/main/resources/application.properties

<pre class="prettyprint highlight" id="code-block-4"><code class="language-java" data-lang="java"><span class="pln">spring</span><span class="pun">.</span><span class="pln">jpa</span><span class="pun">.</span><span class="pln">hibernate</span><span class="pun">.</span><span class="pln">ddl</span><span class="pun">-</span><span class="kwd">auto</span><span class="pun">=</span><span class="pln">create
spring</span><span class="pun">.</span><span class="pln">datasource</span><span class="pun">.</span><span class="pln">url</span><span class="pun">=</span><span class="pln">jdbc</span><span class="pun">:</span><span class="pln">mysql</span><span class="pun">:</span><span class="com">//localhost:3306/db_example</span><span class="pln">
spring</span><span class="pun">.</span><span class="pln">datasource</span><span class="pun">.</span><span class="pln">username</span><span class="pun">=</span><span class="pln">springuser
spring</span><span class="pun">.</span><span class="pln">datasource</span><span class="pun">.</span><span class="pln">password</span><span class="pun">=</span><span class="typ">ThePassword</span></code></pre>
