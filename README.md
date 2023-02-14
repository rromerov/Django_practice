# Hello JP! or anyone else who has accessed this repository

To run this project, just follow these steps:

1. Go to the root folder of the project, in your machine and copy the following on your **CMD** to activate the virtual environment on your computer:

```
env\Scripts\activate
```

2. Then install the modules required for the project:

```
pip install -r requirements.txt
```

3. Now run the project:

```
python manage.py runserver
```

4. Finally open another terminal and copy this: 

```
curl -H "Accept: application/json; indent=4" -u admin:admin http://127.0.0.1:8000/users/
```

**You should the following result:**
```
{
    "count": 1,
    "next": null,
    "previous": null,
    "results": [
        {
            "url": "http://127.0.0.1:8000/users/1/",
            "username": "admin",
            "email": "admin@example.com",
            "groups": []
        }
    ]
}```
