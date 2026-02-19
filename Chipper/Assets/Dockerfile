FROM ubuntu:24.04

# Install C++ runtime library
RUN apt-get update && \
    apt-get install -y libstdc++6 && \
    rm -rf /var/lib/apt/lists/*

WORKDIR /app

# Copy executable
COPY Chipper .

# Make executable runnable
RUN chmod +x Chipper

# Run executable
CMD ["./Chipper"]
