# fastapi-tutorial-mssql
The FastAPI SQL database tutorial modified to use `mssql+pyodbc`.

Proof-of-concept that using FastAPI with mssql does *not* require
aioodbc and `async def` for path operation functions.

See

https://fastapi.tiangolo.com/tutorial/

and

https://fastapi.tiangolo.com/tutorial/sql-databases/

for details on using the tutorial (installing FastAPI,
launching uvicorn, etc.).

GitHub discussion:

https://github.com/sqlalchemy/sqlalchemy/issues/6521

Notes:

- You may need to tweak `SQLALCHEMY_DATABASE_URL` in database.py to connect
to your SQL Server instance.

- This code includes a couple of minor code updates for SQLAlchemy 1.4/2.0.
