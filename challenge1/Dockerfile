# Use the official NGINX image as the base
FROM nginx:alpine

# Remove the default nginx static assets
RUN rm -rf /usr/share/nginx/html/*

# Copy the 'public' directory contents into the container at /usr/share/nginx/html
COPY public /usr/share/nginx/html

# Expose port 80
EXPOSE 80

# Start nginx and keep the process from backgrounding and the container from quitting
CMD ["nginx", "-g", "daemon off;"]
