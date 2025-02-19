# Docker container setup
FROM python:3.9

WORKDIR /app
COPY . /app

RUN pip install --no-cache-dir fastapi uvicorn yfinance numpy pandas scikit-learn tensorflow

CMD ["uvicorn", "stock_api:app", "--host", "0.0.0.0", "--port", "8000"]