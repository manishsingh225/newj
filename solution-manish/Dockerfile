FROM python:3.7

RUN apt-get update
COPY requirements.txt .
RUN pip install -r requirements.txt

WORKDIR /.
COPY app.py .
COPY ./model_data ./model_data/

EXPOSE 8000

CMD ["python", "app.py"]
