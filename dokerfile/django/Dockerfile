FROM python:3.6-slim
COPY ./simple-django-app/cool_counters /app/
WORKDIR /app/
RUN pip install --upgrade pip
RUN pip install django
RUN python manage.py migrate
EXPOSE 8000
CMD ["python", "manage.py", "runserver", "127.0.0.1:8000"]
