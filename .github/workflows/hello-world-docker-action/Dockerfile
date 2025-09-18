# Container image that runs your code
FROM ubuntu-latest

# Copies your code file from your action repository to the filesystem path `/` of the container
RUN apt-get update && \
    apt-get install -y nginx && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

# Expose the default port
EXPOSE 80

# start Nginx in the foreground
CMD ["nginx", "-g", "deamon off;"]
