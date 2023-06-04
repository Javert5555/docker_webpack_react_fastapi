FROM python

# EXPOSE 3000

WORKDIR /api

COPY ./requirements.txt ./app/requirements.txt

RUN pip install --no-cache-dir --upgrade -r ./app/requirements.txt

COPY ./app /api/app

# CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "80"]