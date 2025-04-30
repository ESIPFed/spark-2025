# Use the micromamba base image
FROM mambaorg/micromamba:1.5.0

# Set up the working directory and create a non-root user
WORKDIR /workspace
RUN useradd -ms /bin/bash vscode

# Switch to non-root user
USER vscode