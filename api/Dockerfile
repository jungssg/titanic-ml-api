# 
FROM python:3.9

# 
WORKDIR /code

# 
COPY ./api/requirements.txt /code/requirements.txt

# 
RUN pip install --no-cache-dir --upgrade -r /code/requirements.txt

# 
COPY ./api/api.py /code/

# 
CMD ["uvicorn", "api:api", "--proxy-headers", "--host", "0.0.0.0", "--port", "8000"]
