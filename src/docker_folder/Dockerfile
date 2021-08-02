FROM python:3

WORKDIR /usr/src/app

COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt
# update the latest packages
RUN apt-get update

COPY . .

CMD [ "python", "./main.py" ]