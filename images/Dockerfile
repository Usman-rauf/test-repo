# Use the official NGINX base image
FROM nginx:latest

# Copy custom configuration file to the container
COPY nginx.conf /etc/nginx/nginx.conf

# Set the working directory
WORKDIR /usr/share/nginx/html

# Copy the static HTML files to the container
COPY index.html .

# Expose port 80 for HTTP traffic
EXPOSE 80

# Start the NGINX server
CMD ["nginx", "-g", "daemon off;"]
