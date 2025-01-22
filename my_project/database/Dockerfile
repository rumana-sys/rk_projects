# Use PostgreSQL as the base image
FROM postgres:latest

# Set non-sensitive environment variables
ENV POSTGRES_DB=mydatabase

# Copy the initialization script into the container
COPY init.sql /docker-entrypoint-initdb.d/

# Expose the default PostgreSQL port
EXPOSE 5432

# Define the command to start PostgreSQL
CMD ["postgres"]