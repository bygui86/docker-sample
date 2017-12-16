
# Java parent image
FROM store/oracle/serverjre:8

# Set the working directory to /
WORKDIR /

# Copy the current directory contents into the container at /app
ADD . /

# Install any needed packages specified in requirements.txt
# RUN pip install -r requirements.txt

# Make port 8080 available to the world outside this container
EXPOSE 8080

# Define environment variables
ENV JAVA_PKG server-jre-8u141-linux-x64.tar.gz
ENV JAVA_HOME /usr/java/default

# Run the application when the container launches
CMD ["java", "-jar", "rh-customerservice-0.1.jar"]
