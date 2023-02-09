### Django bookstore

This project follows the Django for Professionals books. The first three chapters are an introduction
and setup and in chapter four we get to create a bookstore project.

To run this application go to `ch4-bookstore` and put up its containers:

```bash
docker compose up -d --build
```

And go to localhost:8000. If you see an error it's because we need to run the migrations:

```bash
docker compose exec web python manage.py migrate
```

For local development, create a virtual environment, activate it and install dependencies:

```bash
python3 -m venv .venv
```

```bash
source .venv/bin/activate
```

```bash
pip install -r requirements.txt
```

Then migrate with the Django manage command:

```bash
python manage.py migrate
```

Finally, run the server:

```bash
python manage.py runserver
```
