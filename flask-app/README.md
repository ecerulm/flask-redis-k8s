

```
poetry install 
poetry run flask -app flask_app run 
poetry run gunicorn -w 2 -b :8000 flask_app
```

```
docker build -t ecerulm/flaskapp:latest . 
docker push ecerulm/flaskapp:latest
docker run -ti --rm -p 8000:8000 ecerulm/flaskapp:latest
```