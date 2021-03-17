This very simple flask project shows the use of the flask-sqlalchemy package for database.  It is does not work as a web app, but allows you to pen a shell and interact with a database.


1. Create and activate virtual environment 
2. `pip install -r requirements.txt`
3. `python`
4. In the Python shell, try these commands

```
from app import db, User
db.create_all()
User.query.all()
user1 = User(username="Yusuf", email="yusuf@gmail.com")
db.session.add(user1)
db.session.commit()
User.query.all()
```

# References

* [Flask-SQLAlchemy Documentation](https://flask-sqlalchemy.palletsprojects.com/en/2.x/quickstart/)
* [Michael Grinberg Flask Mega Tutorial](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-iv-database)