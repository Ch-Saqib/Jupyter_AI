FROM jupyter/base-notebook:latest

WORKDIR /code

COPY . /code/

RUN pip install poetry

RUN poetry configg virtualenvs.create false

RUN poetry install

EXPOSE 8888

CMD [ "jupyter","notebook","--port","8888","--no-browser","--allow-root" ]