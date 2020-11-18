# Building a virtual assistant

- Common chatbot use cases:
    - Scheduling a meeting
    - Etc. 

- Require information about the outside world. 
- Need to interact with databases or API's.

## SQLite in Python

```
import sqlite3

conn = sqlite3.connect('<database>.db')
c = conn.cursor()
c.execute(
    """
        <QUERY>
    """ 
)
```
```
c.fetchall()
```