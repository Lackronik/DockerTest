FROM python:3.9.6-alpine3.13

WORKDIR /usr/src/app/

COPY requirements.txt .

#Create and activate the virtual environment
RUN python -m venv venv && \
    source venv/bin/activate && \
    pip install --no-cache-dir -r requirements.txt

COPY . .

EXPOSE 8080

# Set the entry point to use the virtual environment
CMD ["/usr/src/app/venv/bin/python", "app.py"]
