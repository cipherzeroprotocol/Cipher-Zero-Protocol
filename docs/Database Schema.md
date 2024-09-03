+-----------------+        +-----------------+        +--------------------+
|     User        |        |      File        |        |   Transaction      |
|-----------------|        |-----------------|        |--------------------|
| id (PK)         |        | id (PK)         |        | id (PK)            |
| username        |        | filename        |        | user_id (FK)       |
| email           |        | filesize        |        | file_id (FK)       |
| password        |        | filehash        |        | timestamp          |
+-----------------+        | uploader (FK)   |        +--------------------+
                           +-----------------+
