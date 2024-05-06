# Use a base image with minimal dependencies (e.g., Alpine Linux)
FROM ubuntu:latest

# Set the working directory inside the container
WORKDIR /app

# Copy the compiled server executable into the container
COPY server /app
COPY content.txt /app
COPY server_root/courses/ud923/filecorpus/* /app/server_root/courses/ud923/filecorpus/

# Expose the port your server listens on (replace PORT with the actual port)
EXPOSE 39474

# Command to run the server
CMD ["./server"]

