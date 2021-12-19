FROM rasa/rasa:2.8.1

WORKDIR /app
COPY . /app
COPY ./data /app/data
#COPY ./models /app/models

#RUN pip install rasa==2.8.15
RUN pip install gunicorn==20.1.0
RUN  rasa train

VOLUME /app
VOLUME /app/data
VOLUME /app/models

CMD [ "run","-m","/app/models","--enable-api","--cors","*","--debug" ]