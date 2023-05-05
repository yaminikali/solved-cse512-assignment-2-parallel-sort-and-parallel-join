Download Link: https://assignmentchef.com/product/solved-cse512-assignment-2-parallel-sort-and-parallel-join
<br>
The required task is to build a generic parallel sort and parallel join algorithm.

<ol>

 <li>Implement a Python function <strong>ParallelSort() </strong>that takes as input: (1) <strong>InputTable </strong>stored in a PostgreSQL database, (2) <strong>SortingColumnName </strong>the name of the column used to order the tuples by. <strong>ParallelSort() </strong>then sorts all tuples (using five parallelized threads) and stores the sorted tuples for in a table named <strong>OutputTable </strong>(the output table name is passed to the function). The <strong>OutputTable </strong>contains all the tuple present in <strong>InputTable </strong>sorted in ascending order.</li>

</ol>




<u>Function Interface: –</u>

<strong>ParallelSort (InputTable, SortingColumnName,  OutputTable, openconnection) InputTable – </strong>Name of the table on which sorting needs to be done.

<strong>SortingColumnName  – </strong>Name of the column on which sorting needs to be done, would be either of type integer or real or float. Basically Numeric format. Will be Sorted in Ascending order.

<strong>OutputTable – </strong>Name of the table where the output needs to be stored.

<strong>openconnection – </strong>connection to the database.




<ol start="2">

 <li>Implement a Python function <strong>ParallelJoin() </strong>that takes as input: (1) <strong>InputTable1 </strong>and <strong>InputTable2 </strong>table stored in a PostgreSQL database, (2) <strong>Table1JoinColumn </strong>and <strong>Table2JoinColumn  </strong>that represent the join key in each input table respectively. <strong>ParallelJoin() </strong>then joins both <strong>InputTable1 </strong>and <strong>InputTable2 </strong>(using five parallelized threads) and stored the resulting joined tuples in a table named <strong>OutputTable </strong>(the output table name is passed to the function). The schema of <strong>OutputTable </strong>should be</li>

</ol>

<strong>InputTable1.Column1, InputTable.Column2, …</strong>, <strong>InputTable2.Column1, InputTable2.Column2…</strong>.




<u>Function Interface: –</u>

<strong>ParallelJoin (InputTable1, InputTable2, Table1JoinColumn,  Table2JoinColumn, </strong>

<strong>OutputTable, openconnection)</strong>

<strong>InputTable1 – </strong>Name of the first table on which you need to perform join.

<strong>InputTable2 – </strong>Name of the second table on which you need to perform join.

<strong>Table1JoinColumn  – </strong>Name of the column from first table i.e. join key for first table. <strong>Table2JoinColumn  – </strong>Name of the column from second table i.e. join key for second table.

<strong>OutputTable – </strong>Name of the table where the output needs to be stored.

<strong>openconnection – </strong>connection to the database.




<strong>Naming Convention to be followed strictly:</strong>

Database name – <em>dds_assignment2</em>

Postgres User name – <em>postgres</em>     Postgres password – <em>1234</em>




<strong>Instructions on how this will be tested: –</strong> Please follow these instructions closely.

<ol>

 <li>Two tables would be created in the database manually.</li>

 <li>The created tables would contain at least an integer field, which would be used for both Parallel Sorting and Parallel Joining.</li>

 <li>Then, the ParallelSort() and ParallelJoin() Function would be called to check the correctness of the program.</li>

 <li>Your code should use 5 threads for both ParallelSort() as well as ParallelJoin().</li>

 <li>Your code should be able to handle table irrespective of its schema.</li>

 <li>Do not make your code dependent on any particular table; it should be able to work on any table and any given input columns.</li>

</ol>







<strong>Instructions for Assignment: –</strong>                                                                                                    2

Please follow these instructions closely <strong>else Marks will be deducted.</strong>

<ol>

 <li>Please follow the function signature as provided in the Assignment2_Interfacy.py.</li>

 <li>Please use the same database name, table name, user name and password as provided in the assignment to keep it consistent.</li>

 <li>Please make sure to run the file before submitting and make sure there is no indentation error. In case of any compilation error, 0 marks will be given.</li>

 <li>Do not modify any function signature in Assignment2_Interface.py. In case any modification is needed, please post the same on discussion board.</li>

 <li>For any case of doubt in the assignment, PLEASE USE Discussion Boards, Individual mails would not be entertained.</li>

 <li>Also, It is an individual’s responsibilities to clarify his/her doubts, so read and use Discussion Board extensively.</li>

</ol>





