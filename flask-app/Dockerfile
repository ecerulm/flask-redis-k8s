FROM python:3.11

WORKDIR /usr/src/app

RUN pip install --no-cache-dir -U pip 
RUN pip install poetry

COPY flask_app/ flask_app/
COPY pyproject.toml .
COPY poetry.lock .
COPY README.md . 

RUN poetry install

CMD ["poetry", "run", "gunicorn", "-w", "2", "-b", ":8000", "flask_app:app"]