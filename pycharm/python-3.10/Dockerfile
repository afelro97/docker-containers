FROM python:3.10.8-slim-bullseye
RUN apt update && apt upgrade -y
RUN apt install curl -y
RUN apt install unzip -y
COPY requirements.txt ./
RUN pip install -r requirements.txt
RUN curl -fsSL https://get.deta.dev/cli.sh | sh
ENV PATH="/root/.deta/bin:${PATH}"
EXPOSE 8000
EXPOSE  80



