# Open WebUI - Dockerfile
# Connects to Ollama running on the host machine

FROM ghcr.io/open-webui/open-webui:main

# Expose the web UI port
EXPOSE 8080

# Persistent storage for Open WebUI data
VOLUME /app/backend/data

# Point to Ollama running on the host
ENV OLLAMA_BASE_URL=http://host.docker.internal:11434

# Optional: set a default port (Open WebUI listens on 8080 internally)
# Map it to 3000 on the host via `docker run -p 3000:8080` or docker-compose
