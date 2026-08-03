# Base Image
FROM nginx:latest

# Maintainer (optional but professional)
LABEL maintainer="Adil Khan"

# Remove default nginx web files
RUN rm -rf /usr/share/nginx/html/*

# Copy website files
COPY app/ /usr/share/nginx/html/

# Expose port
EXPOSE 80

# Start nginx
CMD ["nginx", "-g", "daemon off;"]
#CMD ["nginx-invalid"]
