FROM python:latest

# Create app directory
WORKDIR /app

# Copy the files
COPY requirements.txt ./
COPY chat_app.py ./

# Install the dependencies
RUN pip install --upgrade pip
RUN pip install -r requirements.txt

EXPOSE 8501
ENTRYPOINT [ "streamlit", "run", "chat_app.py", "--server.port=8501", "--server.address=0.0.0.0" ]