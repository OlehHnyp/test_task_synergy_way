FROM python:3.8

RUN mkdir -p /usr/src/synergy_way_server/
WORKDIR /usr/src/synergy_way_server/
COPY ./synergy_way_server/ /usr/src/synergy_way_server/

COPY requirements.txt /usr/src/synergy_way_server/requirements.txt
RUN pip install -r requirements.txt

EXPOSE 8000

CMD ["python3", "manage.py", "runserver", "0.0.0.0:8000"]