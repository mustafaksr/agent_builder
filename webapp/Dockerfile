# Use the official Python image as base image
FROM  google/cloud-sdk:latest


# Set the working directory in the container
WORKDIR /app

# Copy the requirements.txt file into the container
COPY ./requirements.txt /app/requirements.txt
COPY . /app

RUN pip3 install --no-cache-dir -r requirements.txt
RUN apt-get install wget unzip nano

EXPOSE 9994

CMD ["python3", "app.py"]
