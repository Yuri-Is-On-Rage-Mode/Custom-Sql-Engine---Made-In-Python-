# Easy Sql (Esql) - The SQL for Dummies Who Can't Handle Real Databases!

## *I was too lazy to learn proper SQL, so I cobbled together this half-assed abomination that I laughably call a database system. It's perfect for "developers" who think Python is hardcore programming. Use it if you dare, suckers!*

> Inflicted upon the world by Me, (Hamza .S) aka (hmZa) - the "genius" who thought this was a good idea

## This steaming pile of code contains:

- `nSqlServerUtil.py`: The main atrocity! Brace yourselves!
- `repl.py`: For masochists who want to interact with this monstrosity directly!
- `codefile.esql`: Basic commands for those who can't handle real SQL syntax!

## "Learn" (If Your Brain Can Handle It)

### *Commands for the Command-Challenged*

- `[-h]` (For when you're too dumb to remember how this crap works)
- `[--serve SERVE]` (Inflict this on a server, because why not?)
- `[--newdb NEWDB]` (Create a new "database" - really just a glorified text file)
- `[--dbpath DBPATH]` (Point to your pathetic excuse for a database)
- `[--newtable NEWTABLE]` (Add another layer to this data lasagna)
- `[--columns COLUMNS [COLUMNS ...]]` (Define columns, as if this were a real database)
- `[--insert INSERT [INSERT ...]]` (Shove some data in there, pray it sticks)
- `[--replace REPLACE [REPLACE ...]]` (For when you screwed up your data entry, again)
- `[--showgrid]` (Admire your handiwork in all its ugly glory)
- `[--grid {json,yaml,toml}]` (Pick your poison for data formatting)
- `[--savetable SAVETABLE]` (Preserve your mistakes for posterity)
- `[--savedb SAVEDB]` (Backup your entire house of cards)
- `[--saveall SAVEALL]` (For the paranoid data hoarders)
- `[--savegrid SAVEGRID SAVEGRID]` (Export your mess to infect other systems)

### *Examples of This Trainwreck in Action*

```ps

PS G:\fri3nds\w-category-projects\JsonSql\Release> python repl.py
>> --newdb db1

>> --newtable UserAccessTokens --columns User_Name Access_Token Quota_Limit Used_Quota User_Type --dbpath ./db1

>> --insert Hamza y877T(Tt*T87tG76T76T76t^& 15000 10090 Premium_User --dbpath ./db1/UserAccessTokens.json

>> --insert Moobi 0xUYT74T37TR4YTYYTYRTY3UG 50000 13090 Premium_User --dbpath ./db1/UserAccessTokens.json  

>> --insert Dude  0x898t76t6T77TtfTFtFTftFt 2000  1900  Free_User    --dbpath ./db1/UserAccessTokens.json    

>> --insert Trump 0x7t58747tr74tr74t37ytryu 2000  1250  Free_User    --dbpath ./db1/UserAccessTokens.json  

>> --showgrid --dbpath ./db1/UserAccessTokens.json
+-------------+---------------------------+---------------+--------------+--------------+
| User_Name   | Access_Token              |   Quota_Limit |   Used_Quota | User_Type    |
+=============+===========================+===============+==============+==============+
| Hamza       | y877T(Tt*T87tG76T76T76t&  |         15000 |        10090 | Premium_User |
+-------------+---------------------------+---------------+--------------+--------------+
| Moobi       | 0xUYT74T37TR4YTYYTYRTY3UG |         50000 |        13090 | Premium_User |
+-------------+---------------------------+---------------+--------------+--------------+
| Dude        | 0x898t76t6T77TtfTFtFTftFt |          2000 |         1900 | Free_User    |
+-------------+---------------------------+---------------+--------------+--------------+
| Trump       | 0x7t58747tr74tr74t37ytryu |          2000 |         1250 | Free_User    |
+-------------+---------------------------+---------------+--------------+--------------+

>> --replace Moobi 0xUYT74T37TR4YTYYTYRTY3UG 50000 13090 Premium_User Moobi 
0xUYT74T37TR4YTYYTYRTY3UG 0 0 Hacker_Dectected --dbpath ./db1/UserAccessTokens.json

>> --showgrid --dbpath ./db1/UserAccessTokens.json
+-------------+---------------------------+---------------+--------------+------------------+
| User_Name   | Access_Token              |   Quota_Limit |   Used_Quota | User_Type        |
+=============+===========================+===============+==============+==================+
| Hamza       | y877T(Tt*T87tG76T76T76t&  |         15000 |        10090 | Premium_User     |
+-------------+---------------------------+---------------+--------------+------------------+
| Moobi       | 0xUYT74T37TR4YTYYTYRTY3UG |             0 |            0 | Hacker_Dectected |
+-------------+---------------------------+---------------+--------------+------------------+
| Dude        | 0x898t76t6T77TtfTFtFTftFt |          2000 |         1900 | Free_User        |
+-------------+---------------------------+---------------+--------------+------------------+
| Trump       | 0x7t58747tr74tr74t37ytryu |          2000 |         1250 | Free_User        |
+-------------+---------------------------+---------------+--------------+------------------+
>>

```

# DEVELOPERS!

### *ONLY ME, (hmZa):*
> Please, This project needs a fix, I am not drunk but you guys deserve better!
> # HAPPY CONTRIBUTE!!!!