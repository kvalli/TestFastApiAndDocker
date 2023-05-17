# 
FROM python:3.10
 
RUN mkdir -p /app

COPY requirements.txt /

RUN pip install fastapi uvicorn 

COPY ./app /app

EXPOSE 8000

CMD ["uvicorn", "app.main:app", "--host=0.0.0.0", "--reload" ,"--port", "8000"]