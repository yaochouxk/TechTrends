FROM python:3.8

WORKDIR /app

COPY ./project/techtrends/requirements.txt ./

RUN pip install -r requirements.txt

COPY ./project/techtrends ./

RUN python ./project/init_db.py

EXPOSE 3111

CMD [ "python", "app.py" ]