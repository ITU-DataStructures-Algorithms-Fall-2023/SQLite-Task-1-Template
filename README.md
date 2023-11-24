# Task-1

**Deadline:** 25-11-2023, 9:00 PM

Read the SQLite specification file for this project before attempting this assignment.
Try to make multiple commits but only a single push to the remote repository.

You have been provided with a sample database `chinook.db`. You're required to implement the `.dbinfo` command of SQLite. Here's the expected output from the real sqlite:

```bash
$ sqlite3 chinook.db .dbinfo
database page size:  1024
write format:        1
read format:         1
reserved bytes:      0
file change counter: 25
database page count: 864
freelist page count: 0
schema cookie:       34
schema format:       1
default cache size:  0
autovacuum top root: 0
incremental vacuum:  0
text encoding:       1 (utf8)
user version:        0
application id:      0
software version:    3007006
number of tables:    13
number of indexes:   11
number of triggers:  0
number of views:     0
schema size:         4677
data version         2
```
You can omit the following fields for now:
- number of tables
- number of indexes
- number of triggers
- number of views
- schema size
- data version

So your output should look something like this:

```bash
$ .\your_sqlite.exe chinook.db .dbinfo
database page size:  1024
write format:        1
read format:         1
reserved bytes:      0
file change counter: 25
database page count: 864
freelist page count: 0
schema cookie:       34
schema format:       1
default cache size:  0
autovacuum top root: 0
incremental vacuum:  0
text encoding:       1 (utf8)
user version:        0
application id:      0
software version:    3007006
```