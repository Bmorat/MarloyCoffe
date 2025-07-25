FROM python:3.12-slim

WORKDIR /app

RUN apt-get update && apt-get install -y curl

COPY . .

RUN curl -Ls https://astral.sh/uv/install.sh | sh && \
    ln -s /root/.local/bin/uv /usr/local/bin/uv

RUN uv pip install --system -r requirements.in

EXPOSE 8082

CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8082", "--reload"]
