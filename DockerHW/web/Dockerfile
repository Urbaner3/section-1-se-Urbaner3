# FROM python:3.11-slim
#
# RUN mkdir /work
# WORKDIR /work
# ADD requirements.txt ./
# ADD main.py
# RUN pip insall -r requirements.txt
#
# CMD ["python", "main.py"]


FROM python:3.9-slim
RUN mkdir /work

WORKDIR /work

COPY requirements.txt /work

RUN pip install --no-cache-dir -r requirements.txt

COPY . /work

EXPOSE 5000

ENV PYTHONUNBUFFERED=1

CMD ["python", "main.py"]
