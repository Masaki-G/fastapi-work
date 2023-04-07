FROM python:3.11.1-slim

WORKDIR /app

COPY requirements.txt .
#/appの中にrequirements.txtをコピー
RUN pip install --no-cache-dir -r requirements.txt 
#requirements.txtの中のものをインストール

COPY fastAPI ./

CMD [ "uvicorn","main:app","--reload","--host","0.0.0.0","--port","8080" ]