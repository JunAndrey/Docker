FROM python:3.8.10
WORKDIR /app
COPY ./requirements.txt /app/requirements.txt
RUN pip3 install --no-cache-dir --upgrade -r /app/requirements.txt
COPY . /app
EXPOSE 6060
ENV venv=venv
CMD ["python3", "manage.py", "runserver", "0.0.0.0:6060"]