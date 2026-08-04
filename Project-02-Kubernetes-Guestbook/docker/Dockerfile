# Use official Nginx base image
FROM nginx:alpine

# Remove default Nginx welcome page files
RUN rm -rf /usr/share/nginx/html/*

# Copy local 'app' folder contents into Nginx html directory
COPY app/ /usr/share/nginx/html/

# Expose port 80 for web traffic
EXPOSE 80

# Start Nginx in the foreground
CMD ["nginx", "-g", "daemon off;"]
