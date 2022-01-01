# fastapi-tutorial-mssql
The FastAPI SQL database tutorial modified to use `mssql+pyodbc`.

Proof-of-concept that using FastAPI with mssql does *not* require
aioodbc and `async def` for path operation functions.

### How to run:

To launch uvicorn:

```
uvicorn sql_app.main:app --reload
```

Then load the fancy interactive docs page at

http://localhost:8000/docs

Details at

https://fastapi.tiangolo.com/tutorial/

and

https://fastapi.tiangolo.com/tutorial/sql-databases/

GitHub discussion:

https://github.com/sqlalchemy/sqlalchemy/issues/6521

Notes:

- You may need to tweak `SQLALCHEMY_DATABASE_URL` in database.py to connect
to your SQL Server instance.