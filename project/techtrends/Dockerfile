FROM python:3.12
LABEL maintainer="Sudhanshu Gangele"

WORKDIR /app

COPY project/techtrends/requirements.txt .
RUN pip install -r requirements.txt

COPY project/techtrends/ .

EXPOSE 3111
RUN python init_db.py

CMD [ "python" , "app.py" ]
