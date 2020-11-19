## Database Normalization
- DB normalization is a process used to organize a database into tables and columns. The main idea with this is that a table should be about a specific topic and only supporting topics included. Take a spreadsheet containing the info as an example, where the data contains salespeople and customers serving several purposes:
- Identify salespeople in your organization
- List all customers your company calls upon to sell a product
- Identify which salespeople call on specific customers
- By limiting a table to one purpose you can reduce the number of duplicate data contained within your database. This eliminates some issues stemming from database modifications.
- To achieve these objectives, we'll use some established rules. As you apply these rules, new tables are formed. The progession from unruly to optimized passes through several normal forms.
- Three normal forms most databases adhere to using. As tables satisfy each successive db normalization form, they become less prone to database modification anomalies and more focused toward a sole purpose or topic. 
## Reasons for Database Normalization
- Three mains reasons to normalize a database: minimize duplicate data, minimize or avoid data modification issues and to simplify queries 
- Table serves many purposes including: Identifying the organization's salespeople, listing the sales offices and phone numbers, associating a salesperson with an sales office, showing each salesperson's customers
## Data Duplication and Modification Anomalies
- Duplicated information presents two problems: it increases storage and decrease performance and it becomes more difficuly to maintain data changes.
- These situations are modification anomalies. Data normalization fixes them. Three modification anomalies 
- The forms are progressive, meaning that to qualify for 3rd normal form a table must first satisfy the rules for 2nd normal form, and 2nd normal form must adhere to those for 1st normal form. Before we discuss the various forms and rules in detail, let’s summarize the various forms:
- *First Normal Form* – The information is stored in a relational table with each column containing atomic values. There are no repeating groups of columns.
- *Second Normal Form* – The table is in first normal form and all the columns depend on the table’s primary key.
- *Third Normal Form* – the table is in second normal form and all of its columns are not transitively dependent on the primary key
